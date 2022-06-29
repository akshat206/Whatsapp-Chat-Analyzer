# A Exhaustive Data Analysis on a WhatsApp Group Chat
## *Overview*

- [Introduction](#introduction)
- [Data Retrieval & Preprocessing](#data-retrieval--preprocessing)
- [Exploratory Data Analysis](#exploratory-data-analysis)

  - **[Overall frequency of total messages on the group.](#the-overall-frequency-of-total-messages-on-the-group)**
  - **[Top 10 most active days.](#top-10-most-active-days)**
  - **[Top 10 active users on the group (with a twist)](#top-10-active-users-on-the-group)**
    - Ghosts present in the group. (shocking results.)
  - **[Top 10 users most sent media.](#the-top-10-users-who-send-the-most-media)**
   - **[Most active hours and days.](#the-top-10-users-who-send-the-most-media)**
    - Heatmaps of weekdays and months.
    - Most active hours, weekdays, and months.
  - **[Most used words - WordCloud](#most-used-words-in-the-whole-chat)**
  
- [Conclusion](#conclusion)

# *Data Retrieval & Preprocessing*
### Beginning. How do I export my conversations? From Where To Obtain Data?

<p align="center">

</p>

- The first step is **Data Retrieval & Preprocessing**, that is to **gather the data**. WhatsApp allows you to **export your chats** through a **.txt format**. 

- Go to the respective chat, which you want to export!

<p align="center">
<img src="https://github.com/akshat206/Whatsapp-Chat-Analyzer/blob/main/assestsw/s2.JPG" width=150 align="center">
</p>

- Tap on **options**, click on **More**, and **Export Chat.**

<p align="center">
<img src="https://github.com/akshat206/Whatsapp-Chat-Analyzer/blob/main/assestsw/s3.JPG" width=150>
</p>

- I will be Exporting **Without Media.**

<p align="center">
<img src="https://github.com/akshat206/Whatsapp-Chat-Analyzer/blob/main/assestsw/s4.JPG " width=200 length=150 align="center">
</p>

### Opening this .txt file up, you get messages in a format that looks like this:

<img src="https://github.com/akshat206/Whatsapp-Chat-Analyzer/blob/main/assestsw/s1.JPG" align="center">

# *Exploratory Data Analysis*

### *Importing Necessary Libraries*

We will be using :
1. **Regex (re)** to extract and manipulate strings based on specific patterns.
    - References:
        - [Regex - Python Docs](https://docs.python.org/3/library/re.html)
        - [Regex cheatsheet](https://www.rexegg.com/regex-quickstart.html)
        - [Regex Test - live](https://regexr.com/)
        - [Datetime Format](http://strftime.org/)
2. **pandas** for analysis.
3. **matlotlib** and **seaborn** for visualization.
4. **emoji** to deal with emojis.
    - References:
        - [Python Docs](https://pypi.org/project/emoji/)
        - [Emoji](https://github.com/carpedm20/emoji)
        - [EMOJI CHEAT SHEET](https://www.webfx.com/tools/emoji-cheat-sheet/)
5. **wordcloud** for the most used words.
6. **datetime** for datetime manipulation.

<p align="center">

</p>

## The overall frequency of total messages on the group

I expect to see a nice line graph with crests and troughs in odd places.
<img src="https://github.com/akshat206/Whatsapp-Chat-Analyzer/blob/main/assestsw/p1.JPG">

## Top 10 Most Active Days
Grouping the data set by date and sorting values according to the number of messages per day.
<img src="https://github.com/akshat206/Whatsapp-Chat-Analyzer/blob/main/assestsw/p2.JPG">

## Top 10 active users on the group

Before analyzing, the top users, let’s find out how many ghosts are there in the group!
<img src="https://github.com/akshat206/Whatsapp-Chat-Analyzer/blob/main/assestsw/p3.JPG">

<img src="https://github.com/akshat206/Whatsapp-Chat-Analyzer/blob/main/assestsw/p4.JPG">

### *Comparing the top 10 users!*

Now, first things first, since almost all the plots will be *comparing one person with another*, I’ll assign a **specific color to each person** so that it becomes **easy to identify each person among multiple plots**.

<p align="center">
<img src="https://github.com/akshat206/Whatsapp-Chat-Analyzer/blob/main/assestsw/p5.JPG">
</p>

#### Let’s see the plots, simultaneously for **some interesting results**!

<p align="center">
<img src="https://github.com/akshat206/Whatsapp-Chat-Analyzer/blob/main/assestsw/p6.JPG">
</p>

## The Top 10 users who send the most media

The exported chats were exported without any media files. Any message that contained media was indicated with *‘<Media Omitted> ’*. **We can use this to filter out and see who sends the most media.**
<p align="center">
<img src="https://github.com/akshat206/Whatsapp-Chat-Analyzer/blob/main/assestsw/p7.JPG">
</p>

### Which hour of the day are most messages exchanged?

<p align="center">
<img src="https://github.com/akshat206/Whatsapp-Chat-Analyzer/blob/main/assestsw/p8.JPG">
</p>

### Visualization

Now, we will be plotting ***grouped by day and respective group by month simultaneously***, to see some interesting results.

<p align="center">
<img src="https://github.com/akshat206/Whatsapp-Chat-Analyzer/blob/main/assestsw/p9.JPG">

### Heatmap of Month sent and Day sent

<p align="center">
<img src="https://github.com/akshat206/Whatsapp-Chat-Analyzer/blob/main/assestsw/p10.JPG">
</p>

## Most Used Words in the whole chat.
<p>
I will be using the `wordcloud` module, to create a WordCloud of the **most used words**! I will be *adding some common words, to the stopwords*, such that it will not be included the WordCloud.
</p>

<p align="center">
<img src="https://github.com/akshat206/Whatsapp-Chat-Analyzer/blob/main/assestsw/p11.JPG">
</p>


## Made with ❤️ By Akshat

