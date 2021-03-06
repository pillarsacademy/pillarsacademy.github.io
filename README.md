# Pillars Academy Website

This is a static website generated by [Jekyll](http://jekyllrb.com/) and hosted using [Github Pages](https://pages.github.com/). Most pages are written in [Markdown](https://guides.github.com/features/mastering-markdown/).

## Updating the main carousel

Update the [carousels data file](https://github.com/pillarsacademy/pillarsacademy.github.io/blob/master/_data/carousels.yml) to modify the list of carousel elements. Each element starts with a hypen as shown in the example below. You can edit the following things for a carousel element:

- image (path to image)
- href (optional, what to link to)

```yaml
- image: /images/slideshow/pa-banner1.jpg
- image: /images/slideshow/pa-banner2014.jpg
  href: http://www.ocif.org
- image: /images/slideshow/pa-banner3.jpg
```

## Updating the menus

Update the [menu data file](https://github.com/pillarsacademy/pillarsacademy.github.io/blob/master/_data/menu.yml) to modify the list of menu elements. Each element starts with a hypen as shown in the example below. You can edit the following things for a menu:

- path
- title to show in the menu
- banner image
- href link if you want the banner to be clickable

```yaml
- path: about
  title: "About"
  banner: /templates/alridah/images/header/missionvision.jpg
  href:
```

Each menu also has a sub-menu that appears below the banner. Just like the menu, these have a path and a title. The menu path must match the folder that the file is in and the item path must match the name of the file (minus the `.md` suffix).

## Creating new events

Click [here](https://github.com/pillarsacademy/pillarsacademy.github.io/new/master/news/upcoming-events/_posts) to open the new events page. You **must** name the filename using the following convention, otherwise your event will not appear. Do not forget the `.md` extension.

`FOUR DIGIT YEAR`-`TWO DIGIT MONTH`-`TWO DIGIT DAY`-`DESCRIPTION SEPARATED BY HYPENS` `.md`

Look at the [existing events](https://github.com/pillarsacademy/pillarsacademy.github.io/tree/master/news/upcoming-events/_posts) before creating a new one. The file content should look the following template:

```
---
layout: event
title: "Thanksgiving Break: No School"
when: 11.27.2014 - 11.28.2014
---

Any additional description here.
```

## Uploading images

Currently the Github web interface does not allow you to directly upload images, so you'll need to use the Github client for Mac or Windows. However, you can also use the following workaround for now:

1. Click [here](https://github.com/pillarsacademy/pillarsacademy.github.io/issues/1) and drag your image to the `Leave a comment box`.
2. Copy the markdown that was generated, you'll paste that wherever you want to put the image later. If you only want the URL (for the carousel for example) just copy everything inside of the parenthesis.
3. Click the `Comment` button to save the comment (this might not be required, the image should still remain even if you don't save the comment).

## Updating the embedded newsletter

1. Click on the "Past Issues" link in the Newsletter section.
2. Right-click on the latest issue, and save the shortcut URL.
3. Paste that copied shortcut in `/news/newsletter.html` to overwrite the existing one.

## Mailing List Subscription Requests

All mailing list signup requests get appended to [this](https://docs.google.com/a/alridah.org/spreadsheets/d/16fhhgdfQyBx2l9pz83JYzieTJIwyPnUe3aBfh1k09_g/edit#gid=647443546) Google Spreadsheet. Contact an administrator if you need to get access to it. You can also add a notification to automatically receive an email when that happens.