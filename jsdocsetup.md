# Purpose

Ho to setup eclipse to support jsdoc

# Prerequisite

* Nodes should be installed
* jsdoc3 should be installed

# Adding JSDoc as an external tool

Create a new external tool configuration in eclipse (name it JSDOC) where:

* <b>location:</b> should be the node executable full path (i.e.: /home/gilbert/.nvm/v0.10.39/bin/node)
* <b>Working Directory:</b> should be the jsdoc directory full path (i.e.: /home/gilbert/.nvm/v0.10.39/lib/node_modules/jsdoc)
* <b>Arguments:</b> jsdoc -r --verbose ${selected_resource_loc} -d ${selected_resource_loc}/out

# To get JSDoc generated

* run the JSDoc external tool
* make sure your project is well selected (some time you get errors because it's not seen as selected... just click 2 or 3 time on your project root and start again)
* after completion, refresh your project to see the out directory where documentation is located
* document any js code according to [how to use JSDoc](http://usejsdoc.org)
* regenerate the documentation when you have changed it (refesh your project at the end...)
* you can open index.htm in the out directory with eclipse browser to see jsdoc documentation
