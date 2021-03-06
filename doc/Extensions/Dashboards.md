source: Extensions/Dashboards.md

# Dashboards
Create customised dashboards in LibreNMS per user. You can share dashboards with other users. You can also make a custom dashboard and
default it for all users in LibreNMS.

Example Dashboard
![Example Dashboard](/img/example-dashboard.png)

### Widgets
LibreNMS has a whole list of Widgets to select from. 
--------------------------------------------------------------
+ Alerts Widget: Displays all alert notifications.
+ Availability Map: Displays all devices with colored tiles, green up, yellow for warning (device has been restarted in last 24 hours),red   for down. You can also list all services and ignored/disabled devcies in this widget.
+ Componet Status: List all componets Ok state, Warning state, Critical state.
+ Device Summary horizontal: List device totals, up, down, ignored, disabled. Same for ports and services. 
+ Device Summary vertical: List device totals, up, down, ignored, disabled. Same for ports and services.
+ Eventlog: Displays all events with your devices and LibreNMS. 
+ External Image: can be used to show external images on your dashboard. Or images from inside LibreNMS.
+ Globe Map: Will display map of the globe.
+ Graph: Can be used to display graphs from devices. 
+ Graylog: Displays all Graylog's syslog entries.
+ Notes: use for html tags, embed links and external web pages. Or just notes in general.
+ Syslog: Displays all syslog entries.
+ Top Devices: By Traffic, or  Uptime, or Response time, or Poller Duration, or Procssor load, or Memory Usage.
+ Top Interfaces: Lists top interfaces by traffic utilization.
+ Worldmap: displays all your devices locations. From syslocation or from override sysLocation.
--------------------------------------------------------------------

List of Widgets: 
![List of Widgets][image of widgets]

[image of widgets]: /img/list-widgets.png "List of the widgets"


### Dashboard Permissions
- Private: Sets the dashabord to only the user that created the dashboard can view and edit.
- Shared Read: Sets the dashboard to allow other users to view the dashboard, but cant make changes to the dashboard.
- Shared: Allows all users to view the dashboard and make changes.

### Setting a global default dashboard
Step 1: Set the dashboard to either shared read or shared, depending on what you want the users access to change. 
Step 2: Then go to Settings -> WebUI settings -> Dashboard Settings and set the global default dashboard.

### Setting embeded webpage
Using the Notes Widget.
```html
<iframe src="url/" width="1200" height="800">
  <p>Your browser does not support iframes.</p>
</iframe>
```
Note you may need to play with the width and height and also size your widget properly.
``` src="url" ``` needs to be URL to webpage your linking to.
Also some web pages may not support html embeded or iframe.
![Example embed webpage](/img/example-embed-website.png)



