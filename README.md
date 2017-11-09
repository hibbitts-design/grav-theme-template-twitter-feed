# Grav Theme Twitter Feed Template and BluePrint

This Template and Blueprint combination provides the ability to include a [Twitter Feed](https:twitter.com) into any Grav Page, with the ability to easily edit the content of an Twitter Feed within the Grav Admin Panel.

## Installing the Template
* Copy the file `twitterwidget.html.twig` to the `templates` folder in your active Theme folder

## Installing the Blueprint
* Copy the file `twitterwidget.yaml` to the `blueprints` folder in your active Theme folder

## Using the Installed Template and Blueprint in the Admin Panel
1. Add a new page, using the `my-twitter-widget` template:
![New Twitter Feed Page](https://github.com/paulhibbitts/github-repo-images/blob/master/twitter-widget-page-add.png?raw=true)  
It is recommend that `Visible` is set to `No` to avoid adding a numeric prefix to the default page filename.  

2. Display the newly created Twitter Feed within a Page, either by using the Page Inject plugin (```[plugin:page-inject](/my-twitter-widget)```) or by using Twig (e.g. ```{{ page.find('my-twitter-widget').content } }}```).

## Editing an Twitter Feed Page in the Admin Panel
![Editing Twitter Feed Page](https://github.com/paulhibbitts/github-repo-images/blob/master/twitter-widget-page-edit.png?raw=true)

## Using the Twitter Feed Template in Page Frontmatter

```
---
title: 'My Twitter Feed'
twitter_feed_text: 'Tweets from @hibbittsdesign'
twitter_feed_url: 'https://twitter.com/hibbittsdesign'
twitter_feed_height: 600
published: true
routable: false
visible: false
---

##### Paul's Twitter Feed
```

## Example Twitter Feed Page
![Example Twitter Feed Page](https://github.com/paulhibbitts/github-repo-images/blob/master/twitter-widget-example.png?raw=true)
