###Function
This function shows numbers of new posts and threads. It accumulates them automatically when you set it.

###Setup
1. \[CC\] -> settings -> Statistics -> Activate (See Pic.1)<br>
2. Reload<br>
3. After reload, you can see 'Graph' in [CC]. Click it. (See Pic.2)<br>
Pic.1 ![Pic.1](https://github.com/DogMan8/CatChan/blob/master/docs/stats_setup_0.png)<br>
Pic.2 ![Pic.2](https://github.com/DogMan8/CatChan/blob/master/docs/stats_setup_1.png)<br>

###Basic settings (See Pic.3)
You can change time time scale or targets using selectors in the title bar, or open settings by clicking 'Gear Mark'.<br>
Time scales: 1 min, 10 mins, 1 hour, 1 day and 1 week.<br>
Select targets: See below.<br>
Settings:<br>
- Number of points: Number of points in graph. 
- Scale of new thread: Scale of new thread. Number of new thread is 10 times or more smaller than new posts usually.
- Shows: Posts/Threads: select which ones to show.
- - Estimated posts: Number of new posts which is estimated from posts' No. This assumes posts' No. are added serially in a board, there are 50 posts between No.1000(referred as >>1000) and No.1050(referred as >>1050). Therefore this doesn't work if the board doesn't gives No. serially. Or sometimes causes spikes when the data are not filled. And this doesn't have granularity of threads; you can't get this number of a thread. 
- - Observed posts: Number of new posts which is observed. This script scans entire board and counts all posts in each thread, and watch all new posts in the board. Sum of these are shown.
- - Alive posts: Number of new posts which are alive. "Observed" - pruned.
- - Observed thread: Number of new threads from the same manner of "Observed posts".
- - Alive thread: Number of new thread from the same manner of "Alive posts".
- Legend: Show legends.
- Animation: Graph animation when new points are added. This doesn't work on FireFox.
- Point dot: radius: You can change point dot and its radius.<br>
Pic.3 ![Pic.3](https://github.com/DogMan8/CatChan/blob/master/docs/stats_settings_0.png)<br>

###Note
You'll see an triangle shape at the first time if you see a fast board like /v/, see Pic.4. The pic tells that all posts before 9:00 are pruned and the script have no clue to estimate before the time. After 9:00 there are some posts alive and the script can estimate coarsely, you can see some spikes. After 16:00 most of all data are filled probably and the estimation will be proper. And several hours later, it will be like pic.5. You can see "observed" and "alive" are split.<br>
Pic.4 ![Pic.4](https://github.com/DogMan8/CatChan/blob/master/docs/stats_note_0.png)<br>
Pic.5 ![Pic.5](https://github.com/DogMan8/CatChan/blob/master/docs/stats_note_1.png)<br>

###Targets selection
###Advanced settings