---
tags:
  - instructions
  - obsidian
  - excalidraw
  - github
creation date: Wednesday 22nd October 2025
---
Practical Benefits of Excalidraw:
- 

#### Make \_assets folder 
Create a folder called  \_assets inside the publish folder in Obsidian for the images to show up on the website (in my case I put it in my docs folder).
1. Right-click over publish docs
2. New Folder
3. Rename to \_assets

#### Hide the \_assets folder from showing up on the website
This finding was from [Growlf](https://growlf.github.io/journal/). Move the \_assets folder into the publish folder and then filter it out of the side menu by editing the relevant line in `quartz_layout.ts`

```
Component.DesktopOnly(Component.Explorer({
      filterFn: (node) => {
        // set containing names of everything you want to filter out
        const omit = new Set(["_assets"])
    
        // can also use node.slug or by anything on node.data
        // note that node.data is only present for files that exist on disk
        // (e.g. implicit folder nodes that have no associated index.md)
        return !omit.has(node.displayName.toLowerCase())
      },
    })),
```
Instructions Contributed By: Vivian, Garth