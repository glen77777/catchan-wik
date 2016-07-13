###Function
CatChan provides keyword search for entire sites. It works as follows basically.<br>
1. Type your keywords in search panel, then threads are filtered by the keyword.<br>
2. If you want to scan posts, boards or sites, click '>' or '>>' to scan. Then scan will start and threads will appear if the keywords are found in the threads.<br>
3. If you want to search continuously, you can set CatChan to store all information of board, boards or sites to get incremental search.<br>
4. If you want to get result popup in catalog, you can set also.<br>

###Basic knowledge of CatChan's search
1. CatChan can filter threads from stored threads and this is all. Therefore you must store them in advance or scan them every time. Threads which fill the criteria will be stored automatically at scan.
2. Most of catalog don't have information about posts in their threads. Therefore you must scan them if you search the keywords from not OP but posts.
3. Index page or some catalog like 4chan have information about posts. Then CatChan's search will seek the keyword from their posts by default. Of course you can change the mode.
4. Filter panel will appear when you click "filter button"(like "Y") in the page.
5. Merged view doesn't have lazy draw control so far, so it's too slow.
6. If you want to see progress of scan, check CC->settings->Networking->"Show details of running indicators"

###Search panel
- Keyword: Root switch for keyword search. It will be active automatically when you start to type keyword.
- Strings: Strings are split by " "(single space) and they are treated as keywords by default.
- Selector: You can select "match all", "match any", "unmatch all" or "unmatch any". Note that "match all" means that the thread has both of any post which matches the keyword. For example, when you set keyword "nagato kusanagi" and search from poster's name, the threads are,
- - match all: "nagato" and "kusanagi" are there.
- - match any: "nagato" or "kusanagi" is there.
- - unmatch all: both "nagato" and "kusanagi" are absent.
- - unmatch any: "nagato" or "kusanagi" is absent. 
- RE: Regular expression.
- CI: Case insensitive, see "A" and "a" as identical letters.
- Sentence: Don't split the keyword by " ", single space is a part of keyword. For example, "Dr. X" without sentence mode matches "Dr. X" and "XERXES" because they are split to "Dr." and "X" by " ". But in sentence mode, it matches "Dr. X" and it doesn't match to "XERXES".
- '>': Scan this board, or these virtual boards if some virtual boards are selected.
- '>>': Scan this site, or all virtual boards if some virtual boards are selected. This scan has limits of maximum number of physical or virtual boards for safe. It's 100 by default.
Pic.search_panel ![Pic.search_panel](https://github.com/DogMan8/CatChan/blob/master/docs/search_panel_0.png)<br>

###Basic Search in catalog
1. Type keywords and set other criteria.
2. If you want to search from posts, click '>' to scan the board, or '>>' to scan entire site.
3. If you want to make next search, type keywords and click scan.

###Stored Search in catalog (incremental posts search)
1. Type keywords and set other criteria.
2. Set the store mode. If you want to store all posts and get popup, see pic.
3. Click '>' to scan the board, or '>>' to scan entire site.
4. Then all posts are stored, you can make next search incrementally.
Pic.stored_search_in_catalog ![Pic.stored_search_in_catalog](https://github.com/DogMan8/CatChan/blob/master/docs/search_stored_catalog_0.png)<br>

###Stored Search in index page (incremental posts search, the same manner as catalog)
1. Type keywords and set other criteria.
2. Index page has the last 5 posts usually, therfore the search seeks the keyword from them by default. If you want to search from all posts in the threads, you must change them, see pic.
3. If you want to scan, click '>' to scan the board, or '>>' to scan entire site.
4. Then all posts are stored, you can make next search incrementally.
5. CatChan also can generate merged view, but it's too slow and it requires reload.
Pic.stored_search_in_index_page ![Pic.stored_search_in_index_page](https://github.com/DogMan8/CatChan/blob/master/docs/search_stored_page_0.png)<br>
