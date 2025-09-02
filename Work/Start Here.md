This is a demo vault for collaboration, knowledge sharing, and project management.  "`= this.file.name`" is the name of this page (note the subtle trick done to get the name within the quotes). This page was last modified at `= this.file.mtime` (note the subtle trick to get the last modified time/date).

I *would* do an Excalidraw to illustrate the directory layout, but it wont stick due to the Relay plugin limitations. So I will simply describe it as best I can.  Everything is in a local vault with a top-level folder named `Work` which is the Relay-shared folder. Within `Work`:

1) `_assets` - Where drawings, media, and other assets *would* go
2) `_templates` - Page templates for folders, content types, and data formatting
3) `Devices` - Every device has a page in here. If it uses voltage and has NET - it has a page
4) `Glossary` - Terms that need extra detail or information that needs to be "somewhere" 
5) `Networks` - Like Devices. Just networks and VLANs
6) `People` - Like Devices. Just people with access
7) `Projects` - again...(you know the deal)
8) `Services` - ...and again
9) Testing - garbage from testing plugins

Outside of this, and thus *not* shared, is my Kanban (and other non-markdown content) and any pre-sharing content that is entirely experimental and not worth sharing yet (if ever).  Settings for the Templater plugin require you to point at the `_templates` folder and to set up the linking of each template to appropriate folders as an automatic before things really start working. This is due to the settings for all of the plugins being kept ***outside*** the shared folder `<vault_path>/Work` - they are kept in the `<vault_path>/.obsidian` folder instead.

# Index

- [[Change Management]] Policy proposal
- [[Project INDEX]] - (see important note about Kanban, below)
- [[Who is Who]]
- [[Services]]
- [[Hardware]]

### Important Notes
- [Dataview docs](https://blacksmithgu.github.io/obsidian-dataview/)
- Kanban (just like anything else that is not Markdown) gets wiped anytime that it syncs up - so I have put a [Kanban page](obsidian://open?vault=RPC&file=KANBAN) ***outside*** the shared folder and point it and the templates correctly within the shared folder - for now, but this only works for local and not collaborative management for the most part.
- For this demo to work with, all content on the local system is in a standard vault with `work` shared (through Relay) at the top level within it. Carefully read the top section and use "common sense" to configure your version to work.  ...for now.

## Top 10 Tasks
In order of priority, auto selected from tasks throughout this vault:
```tasks
not done
sort by priority
limit 10
```
See the [[Project INDEX]] for the full list of tasks.
