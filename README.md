Club Hub
================

See what's next in one glance: Club Hub is a framework that automatically displays event and poster information cleanly and intuitively. It is designed for schools and other organizations with mass comminications needs.
Club Hub also comes with the Synchronized Universal Display (Club Hub SUD), a automated slideshow solution for use on digital displays across campus.
It also integrates into the Club Hub RemindMe! event subscription service, which allows users to get reminders for events.

Download
----------------

Use `git` to pull from this repository:

`git clone https://github.com/geosir/clubhub`

Organization
----------------

The cloned directory contains the following:

1. `frontend`: The code that should be served to the user.
2. `backend`: The Google App Script that should be put in your Google Drive.

Club Hub's frontend is divided into two parts: the main event listing and the Club Hub SUD.

1. The main event listing can be found in the root directory.
2. The Club Hub SUD is located in the `present/` directory. It depends on a few items in `media/`, so if it needs to be moved, then change the includes accordingly.
3. The backend Google App Script code can be found in the `backend/` directory.

Install
----------------

Installing the backend:

1. Make sure you have a Google account with Google App Script that can serve this code.
2. Make the pertinent databses in Google Drive:
	* Make a spreadsheet to use as a Master Event Registry. Make it publicly viewable, and get the document ID.
	* Make a folder to store posters. Make it publicly viewable, and get the document ID.
	* Make a spreadsheet to use as the RemindMe email subscrption registry. Make it publicly viewable, and get the document ID.
3. Upload the contents of `backend/CHER` into a Google App Script document. Put `backend/RemindMe` in another App Script document.
4. Modify these documents as necessary to your liking. Specifically, change the document IDs to the ones found above.
5. Authorize your scripts and get their production links. Save these for use in your frontend installation.

Installing the frontend:

1. Move the contents of the root directory to a folder served by your webserver. Modify it, rebrand it, etc. to your liking...and then you're done!

Protip: You might want to move `backend/` out of the served directory, since it is not used for anything there.

Attribution
----------------

The original idea and framework was formulated, designed, tested, and coded by [George Moe](https://george.moe "George's Website") over the span of nearly two years. Attribution would be very much appreciated.

This work is distributed under a GPLv3 license. See LICENSE for more details.

Contact and Support
----------------

If you have any questions or comments, or if you would like a flavor of Club Hub custom built for your use case, you can contact George Moe at [george@george.moe](mailto:george@george.moe "Email George Moe").
