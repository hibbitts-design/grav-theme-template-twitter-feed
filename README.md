# Grav Theme Twitter Widget Template and BluePrint

This Template and Blueprint combination provides the ability to include a [Twitter Widget](https:twitter.com) into any Grav Page, with the ability to easily edit the content of an Twitter Widget within the Grav Admin Panel.

## Installing the Template
* Copy the file `twitterwidget.html.twig` to the `templates` folder in your active Theme folder

## Installing the Blueprint
* Copy the file `twitterwidget.yaml` to the `blueprints` folder in your active Theme folder

## Using the Installed Template and Blueprint in the Admin Panel
1. Add a new page, using the `my-twitter-widget` template:
![New Twitter Widget Page](https://github.com/paulhibbitts/github-repo-images/blob/master/twitter-widget-page-add.png?raw=true)  
It is recommend that `Visible` is set to `No` to avoid adding a numeric prefix to the default page filename.  

2. Display the newly created Twitter Widget within a Page, either by using the Page Inject plugin (```[plugin:page-inject](/my-twitter-widget)```) or by using Twig (e.g. ```{{ page.find('my-twitter-widget').content } }}```).

## Editing an Twitter Widget Page in the Admin Panel
![Editing Twitter Widget Page](https://github.com/paulhibbitts/github-repo-images/blob/master/twitter-widget-page-edit.png?raw=true)

## Using the Twitter Widget Template in Page Frontmatter

```
---
title: 'My Twitter Widget'
twitter_widget_text: 'Tweets from @hibbittsdesign'
twitter_widget_url: 'https://twitter.com/hibbittsdesign'
twitter_widget_height: 600
published: true
routable: false
visible: false
---

##### Paul's Twitter Feed
```

## Example Twitter Widget Page
![Example Twitter Widget Page](https://github.com/paulhibbitts/github-repo-images/blob/master/twitter-widget-example.png?raw=true)
