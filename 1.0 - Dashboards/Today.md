```tasks
# Only show me tasks that are pending.
not done

# Group these tasks by the file they are in.
group by function task.file.pathWithoutExtension.replaceAll('/', ' / ')

# I am not interested in the following UI elements.
hide created date
hide edit button

# For the UI elements that remain, use icons instead of labels.
short mode
```

# Thoughts & Journal

```dataviewjs
dv.table(
  ["When", "What"],
  dv
    .pages('"7.0 - Thoughts & Journal"')
    .filter(page => page.created || page.updated)
    .map(page => [
      page.created || page.updated,
      page.file.link
    ])
    .filter(page => {
      const then = page[0];
      const today = dv.date('now');

      return then.year === today.year
          && then.month === today.month
          && then.day === today.day;
    })
    .sort(page => page[0], 'asc')
    .map(page => [
      page[0].toFormat('h:mm a'),
      page[1]
    ])
)
```