# OSGI ENROUTE GITHUB ANGULAR-UI

${Bundle-Description}

# Installation

You just need to declare a dependency on the ui.bootstrap module:
angular.module('myModule', ['ui.bootstrap']);
You can fork one of the plunkers from this page to see a working example of what is described here.

## CSS

Original Bootstrap's CSS depends on empty href attributes to style cursors for several components (pagination, tabs etc.). But in AngularJS adding empty href attributes to link tags will cause unwanted route changes. This is why we need to remove empty href attributes from directive templates and as a result styling is not applied correctly. The remedy is simple, just add the following styling to your application:

	.nav, .pagination, .carousel, .panel-title a { cursor: pointer; }

