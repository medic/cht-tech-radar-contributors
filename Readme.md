# CHT Technology Radar for Contributors
This is the location of CHT Technology Radar for Contributors content.

If you are looking for the content of the CHT Technology Radar for Implementers, you can find it [in its dedicated GitHub repository](https://github.com/medic/cht-tech-radar-implementers). 

This Tech Radar is built by using the [CHT Technology Radar Core](https://github.com/medic/cht-tech-radar-core).

## Contribute to the Technical Radar

### Create a new Technology Radar release
For a new Technology Radar release, create a folder of the release date (YYYY-MM-DD) under `./radar`.

### Maintaining content
The items are written in Markdown (`.md`) format.

Each file has a meta header where the attributes of the item are listed:

```
---
title:      "JavaScript"
ring:       adopt
quadrant:   languages-and-frameworks
tags: [frontend, coding]
---

Text goes here. You can use **markdown** here.
```

Following front-matter attributes are possible:

- **title**: Name of the Item
- **quadrant**: Quadrant. One of `languages-and-frameworks` (for `Languages and Frameworks` quadrant),
  `methods-and-patterns`(for `Techniques` quadrant), `platforms-and-aoe-services` 
(for `Platforms` quadrant), `tools` (for `Tools` quadrant)
- **ring**: Ring section in radar. One of `trial`, `assess`, `adopt`, `stop`
- **tags**: Optional tags for filtering.
- **featured**: (Optional, default "true") If you set this to "false", the item
  will not be visible in the radar quadrants but still be available in the overview.

The name of the .md file acts as item identifier and may overwrite items with
the same name from older releases.

If an item is overwritten in a new release, the attributes from the new item are
merged with the old ones, and a new history entry is created for that item.

You can integrate images in your markdown. Put the image files in your public folder and reference them:

```
![an image](/images/an-image.png)
```

### Content Guidelines
You can update the rings and the quadrants in the `config.json` file. If you update the names of the rings and quadrants,
you will need to update the technologies .md files accordingly.

The text on the "How to use the CHT Technology Radar for Contributors" page can be updated in the `about.md` file.

### Customize the radar
> Further instructions on how to customize the Technical Radar can be found in the [medic/cht-tech-radar-core](https://github.com/medic/cht-tech-radar-core) repository.

## Development

### Host the application under a sub path
To host the application under a sub path, set the environment variable `PUBLIC_URL`, e.g. "/cht-tech-radar".
The default is `/`.

> For local development you can use `/build` and use this for the following steps. 

### Build the radar
```
npm install
PUBLIC_URL=/build REACT_APP_RADAR_NAME="CHT Technology Radar for Contributors" npm run start
```

Then open the Tech Radar here: http://localhost:8080/build

### Build the radar with static files
```
npm install
PUBLIC_URL=/build REACT_APP_RADAR_NAME="CHT Technology Radar for Contributors" npm run start:static
```

Then open the Tech Radar here: http://localhost:8080/build

### Regenerate the json file based on your changes on md files
```
npm run generateJson
```

You can do this while the server is running.
You can find the newly created rd.json in `/build/rd.json`.

## Deployment to GitHub Pages
At the moment, the automatic deployment to GitHub Pages via GitHub Actions upon merge to the `main` branch doesn't work. We are trying to find
a solution to this problem via [this ticket](https://github.com/medic/cht-tech-radar-contributors/issues/3).

Until the automatic deployment is solved, please follow the steps below to deploy the latest changes to GitHub Pages.

First, ensure that you are performing the next steps on the `main` branch. 

### Generate the radar with static files
```
PUBLIC_URL=/cht-tech-radar-contributors REACT_APP_RADAR_NAME="CHT Technology Radar for Contributors" npm run build:static
```

### Push the changes to GitHub Pages
```
npm run deploy
```

## Note
The CHT Technology Radars are built starting from the [AOE Tech Radar content](https://www.aoe.com/techradar/index.html).
If you want to build your own Technical Radar you may want to have a look at the [AOE Tech Radar GitHub repository](https://github.com/AOEpeople/aoe_technology_radar).
