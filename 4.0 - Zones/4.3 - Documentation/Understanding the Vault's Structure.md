> [!tldr] What is this?
> This documentation provides a description of what this Obsidian vault is, how it was designed, and information relevant to its intended use. This is starter information, and you are expected to do one of two things: stick with the documentation or make it your own. The goal is to make sure that this document accurately reflects your usage of the vault in case you need to remember how and why things are organized the way they are.

This vault was designed to implement the D.E.E.Z. N.U.T.S. organizational system from [this Reddit post](https://www.reddit.com/r/ObsidianMD/comments/1j66utn/introducing_deeznuts_not_a_meme/). While somewhat jokey in nature, there is genuine value to be found in the way this system suggests content be organized in [[Obsidian]]. If you find that this system does not work for you, you can ~~suck on deez nuts~~ customize this vault or find a more suitable system. The world is your oyster.

# Vault Structure

The vault largely follows the naming convention set by D.E.E.Z. N.U.T.S., but departs from the original "Zettelkasten" folder in favor of "Zones". The reasoning is that the Zettelkasten organization system is antithetical to the use of other organizational systems supported by Obsidian such as folders and tags, both of which are heavily relied on.

## 1.0 - Dashboards

The contents of this folder are notes that are intended to provide a quick, high level view other content in the vault. For example,

- a note could contain a [[Dataview]] query showing all notes that were created in a day
- a note could contain a [[Tasks]] query which shows all pending tasks available
- a canvas is used to link together all related notes on a subject

## 2.0 - Efforts

The contents of this folder are notes related to anything you may be working on and may need to maintain a collection of notes to help keep track of any research or progress made on the effort.

### 2.1 - Projects

This folder is an example of how efforts can be organized. Each folder in this one is expected to be for a separate project. The notes contained within each of the subfolders may be organized in whatever way makes sense for the project. It may make sense to implement the Zettelkasten system separately in each of these project folders.

## 3.0 - Extras

The contents of this folder are largely notes or files that you will rarely, if ever, directly interact with but are still required in order to preserve vault functionality or information that may need be unexpectedly used in the future.

### 3.1 - Templates

This folder contains all of the templates that may be used throughout the vault. Some templates are included with in order to help maintain consistency in how some of the pre-defined folders are populated.

### 3.2 - Archive

This folder contains all of files and notes that are no longer needed (but too afraid to delete), or have yet to be reconciled into the rest of the vault. You may want to exclude this folder when writing Dataview queries, configuring the graph view, or searching for files.

## 4.0 - Zones

The folder primarily exists as a catch all for files and notes that do not cleanly fit into the other primary folders (preserving the acronym). New subfolders may be created as needed in order to better organize content that is needed in the vault.

### 4.1 - Guides

This folder may contain any number of guides on how to complete specific tasks. The included template provides a rough layout for how the guide could be authored and includes suggestions on how it should be read.

### 4.2 - Subjects

This folder is mainly a collection of very simple notes that are intended to be used as back link targets for establishing relationships. The notes themselves should be nothing more than the name of something (e.g. a noun), a short description of what the thing means to you personally, and maybe some additional metadata in the properties. Some examples are included with the vault and are used in this documentation.

### 4.3 - Documentation

This folder, unlike the [[#4.1 - Guides|Guides]] folder, may contain notes that serve as documentation for remembering things rather than acting on anything. However, the documentation may refer to one or more guides if action is required. This note is an example.

## 5.0 - Network & People

The contents of this folder are notes on people and the relationships you personally have with them. It is not intended to serve as a database of contact information (like an address book), but something that can be backlinked to when talking about them in other notes.

### 5.1 - People

This folder is expected to have one note per person in a flat folder structure. It is recommended that you use the person's full name as the name of the note, and then use the `alias` property to link it to more commonly used names (e.g. nick names, pet names, etc.). The body of the note should be a very short description of what they personally mean to you.

### 5.2 - Families

This folder is expected to have one note per [nuclear family](https://en.wikipedia.org/wiki/Nuclear_family) in a flat folder structure. It is recommended that you use the name of the family as the name of the note (e.g. "The Smiths"). If the family is large and spread out geographically, you may also want to append their neighborhood to the name of the note (e.g. "The Smiths of Newbury"). The included template provides a Dataview query that will list all of the people who have the note's link set as their `family` property value.

## 6.0 - Unsorted or Unfinished

As the name implies, the contents of this folder have yet to be sorted into some other part of the vault or have not reached a point where they can be properly organized. The vault is configured to create a new note here by default. Notes in this folder should be short lived or moved as soon as possible.

## 7.0 - Thoughts & Journal

The contents of this folder serves as a dumping ground for all of your thoughts that are either ad hoc and for you personally, or something you want to eventually publish for the world to see.

> [!tip]
> The `CTRL + N` shortcut has been configured to use the "Rapid Note" plugin. After having created the appropriate date folder, you can quickly create a new note using the keyboard shortcut, providing the title of your note, and using `7.x` (replace `x` with the relevant category from below) to suggest the path for the new note.

### 7.1 - Microjournal

> [!info] What is microjournaling?
> This folder is inspired by the [microblogging](https://en.wikipedia.org/wiki/Microblogging) concept, but for personal journal entries.

This folder contains notes for short-form journal entries.

- The notes should be kept in date folders (e.g. `2025/03/09/My New Vault`).
- The use of tags should be inline and not in file properties.
- Custom CSS styling is used to reinforce the idea that notes should be small.

### 7.2 - Journal

This folder contains notes that are long form journal entries. When thoughts and feelings get more complicated than a single paragraph, this is where you will want to put them. The notes should be kept in date folders (e.g. `2025/03/09/Long Story`) and tags should be kept in the `tags` property.

### 7.3 - Microblog

This folder contains notes that may later be published to a microblogging platform.

- The notes should be kept in date folders (e.g. `2025/03/09/My New Vault`).
- The use of tags should be inline and not in file properties.
- No backlinks should be used (they may not work when published).
- Custom CSS styling is used to reinforce the idea that notes should be small.

### 7.4 - Blog

This folder contains notes that may later be published to a blogging platform. The organization of the contents for this folder may be whatever works best for you.

> [!warning] Date Folders
> The idea of using a date folder path was considered, but it did not make much sense considering that the day the note was created may not necessarily be the same day it was published (e.g. spending time doing research, writing, and editing).

### 7.5 - Incidents

This folder contains notes you have gathered to [cover your ass](https://en.wikipedia.org/wiki/Cover_your_ass) and may want to reference again in the future. Each note is expected to begin with a short description of what you are doing, followed by bullets that begin with the time you are writing the note and then the bit of information you would like to remember.

> [!tip] Bullet Time
> You can use the `Alt + Enter` shortcut to quickly create another bullet with time in the note. No need to manually type in the property and time for each update you get for your note!

## 8.0 - Sources

The contents of this folder serve as the source of truth that may be referenced by other notes in the vault. Like the [[#3.2 - Archive|Archive]] folder, these files or notes are rarely used directly and are mostly referenced by other notes.

### 8.1 - Bookmarks

This folder contains very simply notes that primarily contains just the title of the page, a URL to it, and a short description of what the bookmark means to you personally. This is useful when you want to keep track of things you found online but are not worth keeping as bookmarks in your browser.

### 8.2 - Attachments

This folder contains the file attachments that are used by notes in other parts of the vault.