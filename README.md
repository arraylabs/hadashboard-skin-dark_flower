# Dark Flower Skin
Custom skin for HADashboard 2 Beta. This is a work in progress.

![alt tag](/dark_flower.jpg)

##Block Colors

To set individual blocks to different colors use the color variables on the widget_style line. For example:
```
smoke_basement:
  widget_type: sensor
  title: Smoke/CO
  title2: Basement
  widget_style: $red_background
  entity: sensor.smoke_co_basement
```
###Colors available: 
> $orange_background, $red_background, $green_background, $black_background, $blue_background, $brown_background, $purple_background, $white_background

###Changes lost on reload/refresh:
> If you aren't seeing the title text vertically centered in the box then most likely the javascript isn't being run. In your appdaemon.cfg file add the following: ***dash_force_compile = 1***

###Vertical line centering:
> Javascript runs after the dashboard is drawn to vertically center the title blocks for those widgets without title2 text. If the length of the title autowraps the second line it won't look right and it should be manually entered for title and title2.

###Not seeing template or template background?
> You may need to restart HADashboard v2
