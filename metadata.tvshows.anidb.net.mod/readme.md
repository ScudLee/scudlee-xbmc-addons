AniDB.net Scraper for TV Shows [Mod]
====================================
This is a heavily modified version of the AniDB.net TV show scraper.

For support please use the [Kodi forum thread](https://forum.kodi.tv/showthread.php?tid=142835).

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

*   **Delay parameter** - Controls the amount of "busywork" the scraper performs when used.
    Increase this if you find yourself getting banned a lot. (100+ at least).

*   **Anime list URL** - Location of the animetitles.xml used in the title search.
    A more up-to-date version can be found direct from AniDB.net if needed.

*   **Anime mapping URL** - Location of the anime-list.xml that maps shows between 
    AniDB.net and thetvdb.com.

*   **Use personal anime mapping** - If you want to use your own mappings on top of the
    default list, you can.  You only need to include the mappings you wish to change/add to.

*   **Personal anime mapping URL** - Location of your personal mapping list.
    Must be a URL (with protocol).  Direct folder locations won't work.

### AniDB ###

*   **Use official name instead of main name** - This determines the title displayed for the show.

*   **Language** - Which language to use for the official name, and also episode titles and plots.
    The main title will be used if no official title exists in the language chosen.
	Episode details will fallback to English.

*   **Enable prequel lookup** - Only used if the show is not in the mapping list.
    Unlikely you should need to change this.

*   **Alternative prequel link type** - As above.

*   **Return only single Animation studio** - In rare cases multiple studios may be returned.

*   **Treat Secondary characters cast as Main** - Include secondary characters in the main cast for the show.

*   **Map specials at the end of episode list** - Where to list special episodes that don't have positional information.

*   **Map specials inside of episode list** - Whether to use positional information at all.
    (These two settings are independent.)

*   **Keep source line in plot** - Keeps the "Based on..." line (or similar) as the last line of the plot.

*   **Minimum Genre weight** - Categories are weighted on AniDB by how well they fit the show.
    Higher weight = Better fit

*   **Number of Genres returned** - Maximum number of genres returned per show.  
    Actual amount may be lower.

*   **Fetch ratings** - Whether to fetch anidb ratings or not

*   **Rating type** - Either Average or Weighted.  Weighted takes into account ballot-stuffing, so is preferred.

*   **Pre-Krypton ratings** - Use the old rating format (for Gotham or older)

*   **Use tags** - Whether to allow the scraper to automatically add tags for your shows.

*   **Auto-add anime tags to all shows** - Whether to add a specific set of tags to every show.

*   **Use these tags (separate with a semi-colon)** - The specific set of tags to use.  The default is just "Anime",
    but you could for example use: Anime;Animation;Japanese to add all three tags.

*   **Add source-based tags** - Add tags based on any "Original Work" categories.

*   **Source tag prefix** - Prefix to add to source-based tags (to aid in sorting).  Remember to include a space at the end.

*   **Add location-based tags** - Add tags based on any "Location" categories.

*   **Location tag prefix** - Prefix to add to location-based tags (to aid in sorting).  Remember to include a space at the end.

*   **Only use the most precise locations** - Disable to add the entire chain of locations as tags. 
    e.g. Earth->Asia->Japan->Tokyo->Akihabara
	
*   **Add target audience-based tags** - Add tags based on any "Target Audience" categories.

*   **Audience tag prefix** - Prefix to add to target audience-based tags (to aid in sorting).  Remember to include a space at the end.


### TheTVDB ###

*   **Enable fanarts** - Whether to download fanart or not.

*   **Enable extra episode details** - Whether to get episode plot and thumbnails from TVDB