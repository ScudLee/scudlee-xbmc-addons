AniDB.net Scraper for Movies [Mod]
====================================
This is a heavily modified version of the AniDB.net TV show scraper intended for use with movies.

For support please use the [Kodi forum thread](https://forum.kodi.tv/showthread.php?tid=142835).

Settings
--------

### General ###

*   **Use Google Search** - Use Google to perform the initial title search.
    Not as reliable as the default search.

*   **Anime list URL** - Location of the animetitles.xml used in the title search.
    A more up-to-date version can be found direct from AniDB.net if needed.

*   **Anime mapping URL** - Location of the anime-list.xml that maps shows between 
    AniDB.net and thetvdb.com and/or themoviedb.com.

*   **Use personal anime mapping** - If you want to use your own mappings on top of the
    default list, you can.  You only need to include the mappings you wish to change/add to.

*   **Personal anime mapping URL** - Location of your personal mapping list.
    Must be a URL (with protocol).  Direct folder locations won't work.

*   **Delay parameter** - Controls the amount of "busywork" the scraper performs when used.
    Increase this if you find yourself getting banned a lot.

### AniDB 1 ###

*   **Use official name instead of main name** - This determines the title displayed for the movie (and its set).

*   **Official name language** - Which official language to use if the official name is to be used.
    The main title will be used if no official title exists in the language chosen.

*   **Enable prequel lookup** - Only used if the movie is not in the mapping list.
    Unlikely you should need to change this.

*   **Alternative prequel link type** - As above.

*   **Return only single Animation studio** - In rare cases multiple studios may be returned.

*   **Keep source line in plot** - Keeps the "Based on..." line (or similar) as the last line of the plot.

### AniDB 2 ###

*   **Minimum Genre weight** - Categories are weighted on AniDB by how well they fit the movie.
    Higher weight = Better fit

*   **Number of Genres returned** - Maximum number of genres returned per movie.  
    Actual amount may be lower.

*   **Fetch ratings** - Whether to fetch anidb ratings or not

*   **Rating type** - Either Average or Weighted.  Weighted takes into account ballot-stuffing, so is preferred.

*   **Pre-Krypton ratings** - Use the old rating format (for Gotham or older)

*   **Use tags** - Whether to allow the scraper to automatically add tags for your movies.

*   **Auto-add anime tags to all shows** - Whether to add a specific set of tags to every movie.

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

### Movie ###

*   **Enable sets (collections)** - Whether to group movies into sets.

*   **Get set titles from movie set list** - Whether to get the set titles from a manually maintained list
    similar to the mapping list.

*   **Anime movie set list URL** - Location of the movie-set list.

*   **Use personal anime set list** - Like the mapping list, you can also define your own sets
    to add to or override those in the movie-set list.

*   **Personal anime movie set list URL** - Location of your personal movie-set list.
    Must be a URL (with protocol).  Direct folder locations won't work.

*   **Get set titles from themoviedb.org** - Whether to get the set titles from themoviedb.org.
    Can be used in conjunction with the movie-set list.

*   **Prefer themoviedb.org sets** - Movies can only be in one set.  This decides which to use if both themoviedb.org
    and the movie-set list return set titles.

*   **Preferred Certification Country** - Which country's certification rating to use.

### TheTVDB ###

*   **Enable fanarts** - Whether to download fanart or not.


Example Personal Movie-set list
-------------------------------

    <anime-set-list>
      <set>
        <anime anidbid="6432">Lupin Sansei vs Meitantei Conan</anime>
        <titles>
          <title>Lupin Sansei Collection</title>
        </titles>
      </set>
    </anime-set-list>

(The default set for that title is the Conan/Case Closed one.)

###Notes###

*   You don't need to include language information for personal set titles.
*   The movie names are ignored by the scraper, only the anidbid is used.
*   To exclude movies from any set, leave the title blank.
