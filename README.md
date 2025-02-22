Subscribe Button
================

[SubToMe](https://www.subtome.com/) is a **universal subscribe button**.
It decouples the content to which a user can subscribe from the application this user may want to use to perform the subscription.
It's loosely inspired by [WebIntents](http://webintents.org/).

The spec is the code, and the code is open source. Feel free to contribute to it. You could very well run your own instance, but that means users may have to reselect their favorite subscription tool over and over again.

By design, all state is kept in the user's browser, using localStorage.

This is intended to be run as a bookmarklet or an embedded button on any web page.

# Workflow.

1. A user visits a site that is able to provide some kind of subscription mechanism. That web application will then embed in its page some code that will register this application on behalf of the user.

2. The subscription button script will store in the user's session the fact that he can use the previously described app for subscriptions.

3. Later, when on another site which publishes content, the user wants to follow a given resource and clicks on the bookmarklet.

4. The user is then showed the list of services that may be able to handle his subscription.

5. Once the user picks a service, he's sent to that service to complete the subscription.

Check Also
==========

[Ant0ine](http://blog.ant0ine.com/) very kindly contributed a [SubToMe Chrome Extension](https://chrome.google.com/webstore/detail/subtome/cjkhnlmkkfheepafpgppmpdahbjgkjfc). [Source code](https://github.com/ant0ine/subtome-chrome-extension).

[Sören](http://www.soeren-hentzschel.at/) contributed a [SubToMe Firefox extension](https://addons.mozilla.org/en-US/firefox/addon/subtome-subscribe-button/)!

[WordPress plugin](http://wordpress.org/extend/plugins/subtome/). Install it by following [these instructions](http://wordpress.org/extend/plugins/subtome/installation/) or look for `SubToMe` in your WordPress Dashboard's plugin interface.

Todo
====

Check [Github Issues](https://github.com/superfeedr/subtome/issues) for more TODOs

Going Further
=============

We intentionally pushed the complexity down to the subscribing application, which should be smart enough to handle subscriptions if it has registered as such.

The subscribing application is in charge of extracting the data to which the user can subscribe (RSS or Atom feed, Social network handle, ... etc), from the page URL.

Registration for popular readers
================================

Check the [store](https://www.subtome.com/#/store).

Feel free to add yours if you implemented registration. Make sure you support [registration](http://docs.subtome.com/developers/)
as well for your existing users.

Building SubToMe
================

SubToMe uses [Grunt.js](http://gruntjs.com/) for its build process and tests.


Discussions
===========

[The Mozilla Hacks](https://hacks.mozilla.org/2013/02/subtome-a-better-subscribe-button/)

[Zemanta Blog](http://www.zemanta.com/blog/get-more-subscribers-simply/)

Thanks
======
[Ant0ine](http://blog.ant0ine.com/) for the Chrome extension, [Sören](http://www.soeren-hentzschel.at/) for the Firefox extension, [Matthias](http://notizblog.org/) for his help with the WordPress plugin.

