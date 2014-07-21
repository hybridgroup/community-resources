# Pebble Community Resources

We are putting together a collection of community resources for a new section on the Pebble Developer Website, and we need *your* contributions!

There are three types of content we are looking for, **[Example Apps](#example-apps)**, **[Developer Tools](#developer-tools)**, and **[Libraries](#libraries)**.

To add your app, tool, or library to the collection, simply [fork this GitHub repository][1], follow the relevant guide below to create a Markdown file in the right folder, and submit a pull request. 

You can also take a look at some of the apps, tools, and libraries that have already been submitted to see how to do it.

### Example Apps

We are looking for well written apps that other people can use to learn Pebble development.

**NOTE:** You must provide a license for your apps in order for it to get approved. The best way to do that is to include a LICENSE file in your app repository.

To add your app, create a new Markdown file in the `examples` folder with the same name as your app (in a URL friendly style, such as `multi-timer.md` or `uk-transport.md`)

At the top of your Markdown file, you will need to have a metadata block that contains the folllowing properties.

```
---
name: Multi Timer
link: https://github.com/smallstoneapps/multi-timer/
appstore: 52bda40bdc2f4f552e000089
tags:
  - watchapp
  - js
  - storage
---
```

Hopefully `name` and `link` are self explanatory. The `appstore` entry is be the Pebble Appstore ID for your app. If your app isn't on the Pebble appstore, omit this line. The `tags`  property will be used on the site to let people browse by different properties. See below for the list of all of the possible tags.

Below this metadata block you should write a description of your app. Include details of the key features it has.

#### Tags

- `watchapp` - The app is a watchapp.
- `watchface` - The app is a watchface.
- `android` - The app has an Android companion app.
- `ios`- The App has an iOS companion app.
- `js` - The app uses PebbleKitJS
- `pebblejs` - The app is written in Pebble.JS
- `storage` - The app uses Persistent 



### Developer Tools

To add your tool, create a new Markdown file in the `tools` folder with the same name as your tool (in a URL friendly style, such as `watchface-generator.md` or `pebble-local-simulator.md`)

At the top of your Markdown file, you will need to have a metadata block that contains the folllowing properties.

```
---
name: Watchface Generator
link: http://watchface-generator.de
---
```

Below this metadata block you should write a description of your tool.

### Libraries

**NOTE:** You must provide a license for your library in order for it to get approved. The best way to do that is to include a LICENSE file in the repository for your library.

To add your library, create a new Markdown file in the `libraries` folder with the same name as your tool (in a URL friendly style, such as `js-message-queue.md` or `clock-layer.md`).

At the top of your Markdown file, you will need to have a metadata block that contains the folllowing properties.


```
---
name: JS Message Queue
link: https://github.com/smallstoneapps/js-message-queue/
language: js
---
```

The `language` property should be one of `c`, `js`, `android` or `ios`. This will help people find your library.

Below the metadata block you should write a description of your library. Talk about what problem it aims to solve, and how people should use it.

[1]: https://github.com/pebble-hacks/community-resources/fork