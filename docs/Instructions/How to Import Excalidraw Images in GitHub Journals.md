---
tags:
  - instructions
  - obsidian
  - excalidraw
  - github
creation date: Wednesday 22nd October 2025
---
Practical Benefits of Excalidraw:
-  For benefits, check out [[Obsidian Community Plug-Ins]] for more information on Excalidraw

#### Make \_assets folder 
Create a folder called  \_assets inside the publish folder in Obsidian for the images to show up on the website (in my case I put it in my docs folder).
1. Right-click over publish docs
2. Create New Folder
3. Rename to \_assets

#### Create your Excalidraw drawing
1. Right-click over \_assets
2. Create New Drawing
3. Let your creativity take over!

#### Link Excalidraw to other pages
To make images pop up in different pages use the following command:
1. In an Obsidian note, type out: `![[insert_image_name]]`

More information is provided on the official [Obsidian Documentation](https://help.obsidian.md/syntax).
#### Hide the \_assets folder from showing up on the website
This finding was from [Growlf](https://growlf.github.io/journal/). Move the \_assets folder into the publish folder and then filter it out of the side menu by editing the relevant line in `quartz_layout.ts` file from `Component.DesktopOnly(Component.Explorer(),`

To the following code below:
```typescript
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

Instructions Contributed By: [Growlf](https://growlf.github.io/journal/) and Vivian