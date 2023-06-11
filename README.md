# werc-apps-runscript

A [werc](http://werc.cat-v.org/) framework app that runs a script in a subfolder.

## installation and setup

Installation:

* Copy into werc/apps directory in __runscript__ subdirectory.

Setup:

* create any subdirectory in your site directory. Create _werc directory containing config file and a runscript subdirectory.

* put/create your script in _werc/runscript directory

* The _werc/config should contain conf_enable_runscript text with optional script name and an optional pageTitle variable set up

		pageTitle='some title'
		conf_enable_runscript test.rc

* the default script name to run is script.rc unless specified as an optional parameter to conf_enable_runscript

* make sure the script has execution privileges

## usage

The script should echo the content that should be displayed by the plugin. The content should be in html form

## about

A "quick and dirty" app/plugin for werc to run some code and display the results on the web. Developed to read some sensor data.
