# Redmine CORS

Redmine plugin to allow external application to use Redmine REST API with [cross-origin resource sharing, aka CORS](http://en.wikipedia.org/wiki/Cross-origin_resource_sharing).

If you have a browser application that requires access to the Redmine API from a different domain your browser will block the request. This plugin returns the headers expected by the browser to complete request and consume the API.

## Install

Clone the current repo into the `plugins` directory:

```bash
cd $REDMINE_ROOT
git clone git://github.com/smallcubed/redmine_cors.git plugins/redmine_cors
```

and restart webserver to reload the plugins (no need to run any rails scripts for updating the database).

## Setup

In the administration area, click on the *Plugin* section. You need to configure the domains that are allowed to access your REST API. Use `'*'` to allow access from all locations. You can also configure all of the allow headers and methods and set the age as well.

## History

This plugin was created by Marco Vito Moscaritolo (http://github.com/mavimo) and has been updated by (http://github.com/llange) and Fred Cox (http://github.com/mcfedr) as well.
