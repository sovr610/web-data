# web-data
Repository for semi-useful PHP SQL queries you can use to extract useful information from the SWG Oracle database
## Installation
### Settings
To use these scripts on your own site, you'll need to make sure the settings.json file has your specific information set in it.
You do not need to add any properties in this file, you just need to make sure the settings are set right for your instance.

NOTE: Settings is the ONLY FILE YOU NEED TO MAKE CHANGES TO (unless you are on a production server)!  ...and you probably don't
even need to change that one.  However, you will need to change the utils/data file if you are moving your settings file such that
it can find your settings file (that would be on the first line of data.php).

Be sure to PROTECT YOUR SETTINGS.JSON file such that it cannot be accessed from the root folder.  A good way to do this is to
place it in a folder BELOW your root and configure your web server to prevent directory traversing.  If you do place it in a folder
or location below root, remember to update utils/data.php such that it can find your settings file.

### Location
Copy these files to your web server root where they can be accessed.  You can add them to a specific location if you know how to
configure your web server appropriately.  I won't go into how to do that here because of the many different web servers that are
out there and how they're configured.  To make things easy, just copy these files (and utils) directory to the root of your web
server (where your primary home page is located).

## Usage
If you've done everything correctly you should be able to access these files from your web site:

`http://myswgwebsite.com/current-auctions.php`

# Credit
Cekis - Initial creation