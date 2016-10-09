###What is the VirtualBoard?
Virtual board: Virtual board is a tag-based, software-based board system. It aggregates all threads by tags.
OK, let me explain and organize.

Physical board: means a usual board like /a/. This can be accessed by URL directly.<br>
Virtual board: means a bunch of threads which are added specific tags like #a. This can't be accessed by URL directly, but scripts like CatChan will scrape sites to aggregate them. You can switch virtual boards like physical boards.<br>
Tag: means a short word led by "#", like #a, #CatChan or #JavaScript. By default, a thread inherits tags from boards.json and a tag which is the same as board's name. You can add tags in OP or posts by posting word "#XXXX". For example, CatChan thread in lainchan has tags of "#λ"(from board's name), "#XXX", '#XXXX", "#CatChan", "#virtualBoard"(from OP).<br>

###What is the virtue of VirtualBoard?
1. You can merge multiple boards from sites to a catalog.<br>
&emsp;You don't have to visit 4chan/a/, 8chan/a/ and meguca/a/. Or you don't have to see all of 8chan/*pol*/. You can just visit #a or #pol.
2. A thread can exist in multiple virtual boards.<br>
&emsp;You had to decide where your thread should be placed in physical board system. But you can put a thread into multiple boards in virtual board system, so you don't have to decide it. Just make a thread and all users can see them wherever they are. For example, #GamerGate threads are deeply related to #v and #pol, then you can put both tags into OP. Users can see the thread if the users seek #v or #pol. Of course users can filter #v but #pol, then political related threads are removed from #v.
3. Users can move threads to other virtual boards by users' will.<br>
&emsp;When you activate live tag system, tags are extracted from all posts in the thread. Therefore you can add any tags to the thread. This invokes moving thread virtually. Tags are bumped and pruned like threads in a physical board. A thread can have 12 tags by default.
4. Fast and slow threads can coexist in a virtual board.<br>
&emsp;In physical board system, threads in a board are pruned equally. Therefore all threads must have adequate post rate, or pruned immediately. In virtual board system, slow threads and fast threads can coexist as long as they belong to other physical board. Therefore you can see chat thread and deep discussion thread in a catalog. Of course you can sort them by their post rate.
5. You can make subboards easily.<br>
&emsp;The virtual board system is just a filter system technically. They compose a subboard when you put a certain tag to threads in your board. Of course you can seek them from other boards.
6. Virtual board system is a superset of physical board system which is used now.<br>
&emsp;When you limit threads to inherit only a tag which is derived from its board's name, for example, #a for threads in /a/, virtual board system works nearly similar to physical board system. Virtual board system is a superset of physical board system. No features are lost, but it gives extreme flexibility.
7. Good moderation can be provided. Users can evaluate and choose moderators.<br>
&emsp;In physical board system, slow boards are considered as "dead boards", and no one won't post it. Therefore people flock in faster boards, and this pressure can be found everywhere. Moderators are deeply hierarchical, and  their name are concealed. You can't know who moderates which posts. On the contrary, virtual board system is open for participants. Anyone can move any thread to any virtual boards, therefore small "dead board"'s owner can participate to moderate in bigger virtual boards. You may think this brings the same problem that who moderates which thread, but it's not. A thread must belong to a physical board, so you can see who is the moderator by its physical board. You can place your thread to any board in a virtual board system, so you can choose your moderator. If you know a good moderator for the topic, you should put your thread in that physical board with your tag, then you'll get a thread in specific virtual board with a specific moderator. This means virtual board system has evaluation system of moderators inherently. And you can bring good moderators to big board as you wish. Virtual board system keeps moderation granularity small. This brings good moderation potentially.
&emsp;As you understand, physical board means that who is the moderator of this board in virtual board system. We citizen can evaluate the skill of moderators without introducing unnecessary obscuring hierarchy. We can name and evaluate a moderator directly.
8. Give liquidity to trigger appropriate competition between boards or sites by removing barriers.<br>

###How to use it?
&emsp;Virtual boards will appear in boardlist. You can toggle them by clicking it.
Pic.virtualBoard ![Pic.virtualBoard](https://github.com/DogMan8/CatChan/blob/master/docs/vb_boardlist_0.png)<br>
Or you can search and choose virtual boards from search panel manually.
Pic.taglist ![Pic.taglist](https://github.com/DogMan8/CatChan/blob/master/docs/vb_taglist_0.png)<br>

###Set up
&emsp;There are two panels for virtualBoard system, "Virtual Board" and "Live Tag".
- Show virtual boards, up to X: Show virtual boards in boardlist or not, and how many.
- Scan at start up, delay: Xs: Scan sites at start up with X seconds delay.
- Scan targets:
- - None: Don't scan.
- - Board: Read boards.json to know which boards are there, and add board's tag.
- - Thread: Scan whole boards to know tags in threads.
- - Instant scan: Scan immediately after changing scan targets.
- Physical boards in boardlist: determine how to handle physical boards in boardlist.
- Show information hover: Show tag's information on hover.
- - U: urty/ur/urt / T: nt / B: snb/nb
- - urty: number of unread replies to you in threads which have this tag.
- - ur: number of unread replies in threads which have this tag.
- - urt: number of threads which have unread replies in threads which have this tag.
- - nt: number of threads which have this tag.
- - snb: number of scanned boards which have threads which have this tag.
- - nb: number of boards which have threads which have this tag.
- Style of selected board: style of selected board in boardlist or each thread.
- Add style: Change tag's style according to tag's state.<br>
Pic.setting_virtualBoard ![Pic.setting_virtualBoard](https://github.com/DogMan8/CatChan/blob/master/docs/vb_setup_vb_0.png)<br>
- From: Choose source of extraction of tags, OP or whole posts in a thread.
- Live: Update tags lively.
- max: max number of tags in a thread.
- max string length: max length of each tag.
- Case insensitive: Case insensitive about tag.
- Click function: Choose function at click the tag.
- - Pickup: pick up threads which have the tag. 
- - Include: show threads which have the tag.
- - Exclude: hide threads which have the tag.<br>
Pic.setting_liveTag ![Pic.setting_liveTag](https://github.com/DogMan8/CatChan/blob/master/docs/vb_setup_lt_0.png)<br>
