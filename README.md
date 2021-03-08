# About this repo

I have pulled a fork to build it for my needs. There is not much in it yet, but it will come.

* Integration into other systems (Contao)
    * Namespaces or even wrapping into a class
* Support of API V1 (ajax) as well as API V2 (REST)
    * It is a bit a problem that domain already has the query in it
* Playground to play around with the API
* More documentation
* Improve Handling of the credentials   
* use https://github.com/guzzle/guzzle

# CT-API-Tools
PHP scripts, that make imports via the ChurchTools API or similar very easy.

## cthelper.php
You need to do something special with the API of CT on your own?
Have a look, maybe I've already discovered, how some part of the API works. You might find the fitting API call in this file!

## ctimportsongs.php

Provides functionality to import a bunch of [OpenLyrics](https://openlyrics.org) xml song files automagically to ChurchTools.
All you need to do is:
- add your login data in the `ctimportsongs.php` file (search for `ToDo`
- have php installed (command line support is *highly* recommended
- copy your OpenLyrics files to the `songs` folder
- in the terminal (CMD on Windows) run: `php ctimportsongs.php`
- now all songs from the `songs` folder should be automagically uploaded to your ChurchTools instance

## ctinvtagstogroup.php

A utility to remove tags from persons and instead add them to a group... only use if you know what you're doing.
The tag and group ids have to be replaced in the file before using.

## calendarmerger.php

You want to subscribe two ical sources, but only have limited calenders booked @CT?
With the calendarmerger you can just host this file on a webserver, add your ical urls, you would like to subscribe to.
Now you can add the URL to the webserver you are hosting this on (e.g. `https://my-super-cool-domain.tld/calendarmerger.php`) 
to ChurchTools as an iCal source and voilá: CT shows both calendars as one.

## ctgetallresourcebooking.php

this generates the ressourcebookings of the day as html file - to be used for digital signeage.

# More information

* https://intern.church.tools/?q=churchwiki#WikiView/filterWikicategory_id:0/doc:API/follow_redirect:true/
* https://api.church.tools/


