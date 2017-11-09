# Grav Theme Twitter Feed Template and BluePrint

This Template and Blueprint combination provides the ability to include a [Twitter Feed](https:twitter.com) into any Grav Page, with the ability to easily edit the content of an Twitter Feed within the Grav Admin Panel.

## Installing the Template
* Copy the file `twitterfeed.html.twig` to the `templates` folder in your active Theme folder

## Installing the Blueprint
* Copy the file `twitterfeed.yaml` to the `blueprints` folder in your active Theme folder

## Using the Installed Template and Blueprint in the Admin Panel
1. Add a new page, using the `Twitterfeed` template:
![New Twitter Feed Page](https://github.com/paulhibbitts/github-repo-images/blob/master/twitter-feed-page-add.png?raw=true)  
It is recommend that `Visible` is set to `No` to avoid adding a numeric prefix to the default page filename.  

2. Display the newly created Twitter Feed within a Page, either by using the Page Inject plugin (```[plugin:page-inject](/my-twitter-feed)```) or by using Twig (e.g. ```{{ page.find('my-twitter-feed').content } }}```).

## Editing an Twitter Feed Page in the Admin Panel
![Editing Twitter Feed Page](https://github.com/paulhibbitts/github-repo-images/blob/master/twitter-feed-page-edit.png?raw=true)

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
![Example Twitter Feed Page](https://github.com/paulhibbitts/github-repo-images/blob/master/twitter-feed-example.png?raw=true)
