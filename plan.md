#RGSoC Projectplan❤Team Delta Quadrant

##What we could work on

###Show geo-location on a osm-map:
* https://github.com/diaspora/diaspora/issues/5813

*why we chose that issue:* we already worked on heatmap layers on osm maps with a javascript library and are interested in transferring a similar concept into ruby, Julia has also a lot of experience in working with maps due to her job at the HERE

*learning expectancy:* learning more about geolocation data and about representing them visually, implement a new feature into a complex software architecture, thinking how to implement that feature in the context of possible privacy issues and opt out wishes by users

###Use chunking to upload photos:
* https://github.com/diaspora/diaspora/issues/4997

*why we chose that issue:* we know similar problems in other apps we work on and find it interesting to figure out possible solutions for that issue. Since diaspora pods all have different configurations it can be vital especially for smaller pods to improve the image upload to prevent timeouts.

*learning expectancy:* getting to know different possibilities for picture upload and their differences, learn more about the concept of chunking and how it works, learning to change and refactor already existing features and clean up code that is not needed anymore afterwards 

###Create a new role: Moderator
* https://github.com/diaspora/diaspora/issues/5324

*why we chose that issue:* this is a complex issue that needs a concept of rights management, a deep understanding of the processes in the app to understand which tasks a moderator should work on and which processes are restricted, we also think the details of the moderation rights should be discussed in the diaspora development community  

*learning expectancy:* getting to know the existing structure of rights management, learning to add new database migrations to assign new role to certain people, create a workflow for decision making (Who will be a moderator?) and to issue the right (e.g. via admin interface)  

####We are also interested in working with APIs to export from and import to diaspora* (focus on tumblr):
* Implement better automatic formatting of outbound posts to Tumblr 
 * https://github.com/diaspora/diaspora/issues/5397 

*why we chose this issue:* we are interested in data transaction of every kind, so the deeper work on the tumblr API and the import and export into diaspora and the problems connected to it  

*learning expectancy:* getting to know the tumblr API and the interaction with diaspora, learning about the possibilities and restrictions that come with that API

###We also propose:
to create a docker file or vagrant file for the development environment to make it easier for us and potential new contributors to get started

##Goals:
* understand the architecture of diaspora* and the structures of discussion and decision making in the diaspora* developer community
* being able to add small features and to improve some processes

##Timeline

* 1st Week
 * read FAQ for developers and related discussions & get familiar with the project
 * setup development environment
   * investigate the needs for setting up the diaspora development environment 
   * investigate the creation of a docker or vagrant file for easy setup
   * set up the development environment
 * get familiar with RSpec & Cucumber test environment
* 1st Month
 * Start working on our first issue on showing geo-locations on an osm-map
   * doing research on how other services use geo-location in their posts
   * investigate the OSM API and Map Libraries like Leaflet
   * discuss the concept of possible opt out to this feature and find a solution to do so
   * implement tests and process to make map visualization of current geo-location work  
  * get used to working as a team with git (merge conflicts, branching, …)
 * finish our work on showing geo-locations and make the first pull request!
* 2nd Month
  * solve issues:
   * to use chunking to upload photos
     * look at other chunking upload solutions
     * build mini app to test different solutions and understand the upload logic used in diaspora
     * implement chunking to upload photos into diaspora* and make a pull request
   * Create a new role: Moderator 
    * evaluation of possible rights of a moderator 
    * discussion in the active developer community (using Github and IRC)
    * design and implementation of the feature and make a pull request
* 3th Month
 * if there is still time work on exchanging content to and from tumblr
   * investigate the existing Tumblr connection in diaspora & the Tumblr API
   * implement better automatic formatting of outbound posts to Tumblr 
   * create pull request


