# Release History

* 20190328, V0.0.24
    * Added node v10 build to travis build regime
    * Added note about unsupported SP-2101W V2, issue #14
    * Dependency updates
    * Revised Copyright Notice
    
* 20170218, V0.0.23
    * Dependency updates
    * Revised Firmware Downgrade Guide and Copyright Notice
    
* 20171218, V0.0.22
    * Dependency updates
    * Updated Travis build descriptor
    * Revised README, added incompatibility notice
    * Added Firmware Downgrade Guide
    
* 20171204, V0.0.21
    * Dependency updates

* 20170514, V0.0.20
    * Fix: Syntax Error. Misplaced semicolon result in globals
    
* 20170404, V0.0.19
    * Feature: Added a private HTTP connection agent as using the global agent may have undesirable side effects
      in application with multiple connection targets
    * Fix: Use util.inspect instead of JSON.stringify to avoid circular dependencies error if debugging is enabled
    * Updated and revised dependencies. Now using Object.assign instead of lodash assign

* 20170029, V0.0.18
    * Feature: Added support for digest authentication required with firmware versions SP-2101W v2.08 and SP-1101W v2.04
    * Integrated modified version of http-digest-auth with fallback to basic authentication to
      support older firmware versions

* 20170118, V0.0.17
    * Feature: Added method to get the current schedule state (contributed by @mplessing)
    * Dependency updates
    
* 20161207, V0.0.16
    * Dependency updates
    * Revised README
    * Updated Travis build descriptor
    
* 20160831, V0.0.15
    * Feature: Added method to access history data (contributed by @mattjgalloway)
    * Updated README and demo.js
    * Dependency updates
    
* 20160503, V0.0.14
    * Bug fix: Close discovery socket on error
    * Improved error handling
    
* 20160503, V0.0.13
    * Fix: ensure discovery service will timeout if no results received

* 20160425, V0.0.12
    * Added device discovery service
    * Dependency updates
    * Replaced lodash with lightweight lodash method modules
    * Added release history file
    * Updated README
    
* 20160305, V0.0.11
    * Dependency updates
    * Replaced deprecated use of Promise.settle()
    * Minor changes of demo.js

* 20151231, V0.0.10
    * Added missing commit from previous releas
    
* 20151231, V0.0.9
    * Bug fix. Always set SmartPlug id XML-Attribute to "edimax" rather than the name assigned to the plug.
    * Dependency update
    * Added basic Travis builds
  
* 20150511, V0.0.8
    * Enforce a default timeout of 20000 msecs to cleanup if client is connected but server does not send a response.

* 20150508, V0.0.7
    * Fixed request error handling. Request must be aborted if error has occurred
    * Added option to set a request timeout
    
* 20150416, V0.0.6
    * Fixed bug in request processing which caused a TypeError if withMetering was set to false

* 20150413, V0.0.5
    * Added getStatusValues() method to provide bulk updates optionally including metering values
    
* 20150413, V0.0.4
    * Improved error handling (Unauthorized case, in particular)
    * Handle chunked response data
    * Added basic implementation to obtain schedule info
    * Updated README
    
* 20150413, V0.0.3
    * Added function to get Energy & Power attributes and to read device information (vendor, model, firmware version)
    
* 20150412, V0.0.2
    * Corrected package descriptor
    
* 20150412, V0.0.1
    * Initial Version
