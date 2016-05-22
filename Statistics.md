###Function
This function shows numbers of new posts and threads. It accumulates them automatically when you set it.

###Setup
1. \[CC\] -> settings -> Statistics -> Activate (See Pic.1)<br>
2. Reload<br>
3. After reload, you can see 'Graph' in [CC]. Click it. (See Pic.2)<br>
Pic.1 ![Pic.1](https://github.com/DogMan8/CatChan/blob/master/docs/stats_setup_0.png)<br>
Pic.2 ![Pic.2](https://github.com/DogMan8/CatChan/blob/master/docs/stats_setup_1.png)<br>

###Basic settings (See Pic.3-1, 3-2)
You can change window size by grabbing right bottom corner of the window though it's really hard to grab. And you can change time scale or targets using selectors in the title bar, or open settings by clicking 'Gear Mark'.<br>
Time scales: 1 min, 10 mins, 1 hour, 1 day and 1 week.<br>
Select targets: See below.<br>
Settings:<br>
- Number of points: Number of points in graph. 
- Scale of new thread: Scale of new thread. Number of new thread is 10 times or more smaller than new posts usually.
- Shows: Posts/Threads: select which ones to show.
- - Estimated posts: Number of new posts which is estimated from posts' No. This function assumes that posts' No. are added serially in a board; there are 50 posts between No.1000(referred as >>1000) and No.1050(referred as >>1050). Therefore this function doesn't work if the board doesn't give No. serially. Or sometimes causes spikes when the data are not filled. And this doesn't have granularity of threads; you can't get this number of a thread.
- - Clip posts: As stated above, estimated numbers may cause spikes, so you can clip them. See difference between Pic.3-1(clipped) and Pic.3-2(raw). 
- - Observed posts: Number of new posts which is observed. This script scans entire board and counts all posts in each thread, and watch all new posts in the board. Sum of these are shown.
- - Alive posts: Number of new posts which are alive. "Observed" - pruned.
- - Observed thread: Number of new threads from the same manner of "Observed posts".
- - Alive thread: Number of new thread from the same manner of "Alive posts".
- Legend: Show legends.
- Animation: Graph animation when new points are added. This doesn't work on FireFox.
- Point dot: radius: You can change point dot and its radius.<br>
Pic.3-1 ![Pic.3-1](https://github.com/DogMan8/CatChan/blob/master/docs/stats_settings_3.png)<br>
Pic.3-2 ![Pic.3-2](https://github.com/DogMan8/CatChan/blob/master/docs/stats_settings_4.png)<br>

###Note
You'll see an triangle shape at the first time if you see a fast board like /v/, see Pic.4. The pic tells that all posts before 9:00 are pruned and the script have no clue to estimate before the time. After 9:00 there are some posts alive and the script can estimate coarsely, you can see some spikes. After 16:00 most of all data are filled probably and the estimation will be proper. And several hours later, it will be like Pic.5-1, 5-2. You can see "observed" and "alive" are split. And you'll get Pic.6 finally.<br>
Pic.4 ![Pic.4](https://github.com/DogMan8/CatChan/blob/master/docs/stats_note_0.png)<br>
Pic.5-1 ![Pic.5](https://github.com/DogMan8/CatChan/blob/master/docs/stats_note_1.png)
Pic.5-2 ![Pic.5](https://github.com/DogMan8/CatChan/blob/master/docs/stats_note_3.png)<br>
Pic.6 ![Pic.6](https://github.com/DogMan8/CatChan/blob/master/docs/stats_note_2.png)<br>

###Targets selection (See. Pic.7)
You can set targets using board groups. The first board group is base board; when you in /v/, it is /v/. Therefore you can see graph of each board by visiting each board. But the second and later board group are configurable and you can switch it instantly. The first column is a label, the second and later column are targets. You can add '!stat' to accumulate data of the board group automatically. As you see in Pic.4, data must be accumulated if you want to see data of long time ago of fast boards. The numbers are summed in a board group. You can see numbers of a thread when you set a thread to a board group.<br>
Pic.7 ![Pic.7](https://github.com/DogMan8/CatChan/blob/master/docs/stats_settings_1.png)<br>

###Advanced settings (See Pic.8)
- Take statistics: Taking statistics, this consumes memory and CPU. Turn off when you don't need this function.
- Estimate num of...: Activate estimation from posts' No., this also consumes memory and CPU. Turn off when you don't need this function.
- Accumulation: Settings of accumulation.
- Tolerant of ...: This function will work when your local clock is not accurate, but it wastes CPU power. You should set it accurate.<br>
Pic.8 ![Pic.8](https://github.com/DogMan8/CatChan/blob/master/docs/stats_settings_2.png)<br>

###Popup chart of individual thread (See Pic.9-1, 9-2)
You can get popup chart of individual thread when you are in catalog. Popup chart doesn't have any individual settings, all settings are inherited from default. See Pic.8<br>
Pic.9-1 ![Pic.9-1](https://github.com/DogMan8/CatChan/blob/master/docs/stats_popup_0.png)
Pic.9-2 ![Pic.9-2](https://github.com/DogMan8/CatChan/blob/master/docs/stats_popup_1.png)<br>

