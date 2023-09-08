# CHT Technology Radar for Contributors

This is the location of CHT Technology Radar for Contributors content.

## Content Guidelines

New blips should be tagged. The following tags are currently established:

* data
* dashboards
* etc.

e.g. use like this:

```md
tags: [data, dashboards]
```

## Development

### Host the application under a sub path
To host the application under a sub path, set the environment variable `PUBLIC_URL`, e.g. "/techradar".
The default is `/`.

> For local development I recommend using `/build` and use this for the following steps. 

### Build the radar
```
npm i
PUBLIC_URL=/build REACT_APP_RADAR_NAME="CHT Technology Radar for Contributors" npm run start
```

Then open here: http://localhost:8080/build

### Build the radar with static files
```
npm i
PUBLIC_URL=/build REACT_APP_RADAR_NAME="CHT Technology Radar for Contributors" npm run start:static
```

Then open here: http://localhost:8080/build

### Regenerate the json file based on your changes on md files
```
npm run generateJson
```

You can do this while the server is running.
You can find the newly created rd.json in "/build/rd.json". 

# Note
The CHT Tech Radars are built starting from the [AOE Tech Radar content](https://www.aoe.com/techradar/index.html).
If you want to build your own Tech Radar you may want to have a look at [AOE Tech Radar GitHub repository](https://github.com/AOEpeople/aoe_technology_radar).

