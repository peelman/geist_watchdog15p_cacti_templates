OVERVIEW
--------

This is a collection of scripts and Cacti templates to graph the output from [Geist Watchdog 15p](http://www.itwatchdogs.com) systems.  

I have included a host template, data templates, and the necessary snmp_query files for T3HD sensors and RTAFHD3 sensors. If you are using other Geist sensors, and create your own query files for them, please consider sending a pull request to add them here.

The Cacti templates have all been exported from Cacti 0.8.8a.

Importing into newer versions of Cacti should work, but importing into previous versions of Cacti will probably not work - if you have problems with the templates, please try upgrading first before reporting a bug.

INSTALLATION
------------

1. Copy snmp_queries/geist\_*.xml to your Cacti server, and place it
under `<cacti_path>/resource/snmp_queries`. Under Debian/Ubuntu, this is
`/usr/share/cacti/resource/snmp_queries`, but may be different for other systems.
1. Log into your Cacti web interface, and click on "Import Templates". Import
the template in the templates directory.

You should then be able to go to the host device you want to monitor, and add the new data queries. Then, click on "Create Graphs for this Host", and select the devices you want to graph.


FEEDBACK
--------
Any comments, criticism, bug reports, suggestions, fixes, etc. all appreciated!
