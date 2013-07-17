AniDB.net Scraper for TV Shows [Mod]
====================================
This is a heavily modified version of the AniDB.net TV show scraper.

For support please use the [XBMC forum thread](http://forum.xbmc.org/showthread.php?tid=142835).

(Extra) Special Episodes
------------------------
OPs/EDs, trailers, and more can be treated as special episodes.  Just start numbering them from 100+.

|    Type     |     Episode number      |
| ----------- | ----------------------- |
|OPs/EDs  "C" |Season 0 Episodes 101-199|
|Trailers "T" |Season 0 Episodes 201-299|
|Parodies "P" |Season 0 Episodes 301-399|
|Other    "O" |Season 0 Episodes 401-499|

Settings
--------

### General ###

*   **Use Google Search** - Use Google to perform the initial title search.
    Not as reliable as the default search.

*   **Store anime ID from** - Site to store the ID from.  Either AniDB.net or thetvdb.com.
    Use thetvdb.com if you use the extra fanart downloader.

*   **Anime list URL** - Location of the animetitles.xml used in the title search.
    A more up-to-date version can be found direct from AniDB.net if needed.

*   **Anime mapping URL** - Location of the anime-list.xml that maps shows between 
    AniDB.net and thetvdb.com.

*   **Use personal anime mapping** - If you want to use your own mappings on top of the
    default list, you can.  You only need to include the mappings you wish to change/add to.

*   **Personal anime mapping URL** - Location of your personal mapping list.
    Must be a URL (with protocol).  Direct folder locations won't work, but file:/// protocol does.

*   **Delay parameter** - Controls the amount of "busywork" the scraper performs when used.
    Increase this if you find yourself getting banned a lot. (100+ at least).

### AniDB 1 ###

*   **Use official name instead of main name** - This determines the title displayed for the show.

*   **Official name language** - Which official language to use if the official name is to be used.
    The main title will be used if no offcial title exists in the language chosen.

*   **Enable prequel lookup** - Only used if the show is not in the mapping list.
    Unlikely you should need to change this.

*   **Alternative prequel link type** - As above.

*   **Return only single Animation studio** - In rare cases multiple studios may be returned.

*   **Treat Secondary characters cast as Main** - Include secondary characters in the main cast for the show.

*   **Map specials at the end of episode list** - Where to list special episodes that don't have positional information.

*   **Map specials inside of episode list** - Whether to use positional information at all.
    (These two settings are independent.)

### AniDB 2 ###

*   **Minimum Genre weight** - Categories are weighted on AniDB by how well they fit the show.
    Higher weight = Better fit

*   **Number of Genres returned** - Maximum number of genres returned per show.  
    Actual amount may be lower.

*   **Use rating** - Either Average or Weighted.  Weighted takes into account ballot-stuffing, so is preferred.

*   **Use tags** - Whether to allow the scraper to automatically add tags for your shows.

*   **Auto-add anime tags to all shows** - Whether to add a specific set of tags to every show.

*   **Use these tags (separate with a semi-colon)** - The specific set of tags to use.  The default is just "Anime",
    but you could for example use: Anime;Animation;Japanese to add all three tags.

*   **Add source-based tags** - Add tags based on any "Original Work" categories.

*   **Source tag prefix** - Prefix to add to source-based tags (to aid in sorting).  Remember to include a space at the end.

*   **Add location-based tags** - Add tags based on any "Location" categories.

*   **Location tag prefix** - Prefix to add to location-based tags (to aid in sorting).  Remember to include a space at the end.

*   **Add tags from AniDB** - Whether to use the tags used on AniDB.

*   **Minimum Approval for tags** - Similar to genre weight.  Higher approval = Better fit.

*   **Include spoiler tags** - SPOILER ALERT!

### TheTVDB ###

*   **Enable fanarts** - Whether to download fanart or not.

*   **Continue lookup if no fanart found** - Only used if the show is not in the mapping list.
    Determines whether to continue searching TVDB if the first match has no fanart.

*   **Enable extra episode details** - Whether to get episode plot and thumbnails from TVDB