# yourmotheris-data

## UPDATE: Discord Server
Join the [Your Mother Bot Official Server](https://discord.gg/NGKSCxyXtq), which features a bot made by [noobyfato](https://github.com/noobyfato)! You can add the announcement channels with updates to your own server.

## yourmotheris-data
Data for the hourly Your Mother Is word.

## Accessing data
[current.txt](https://raw.githubusercontent.com/ajlee2006/yourmotheris-data/main/current.txt) gives JSON data of the latest word. [past.txt](https://raw.githubusercontent.com/ajlee2006/yourmotheris-data/main/past.txt) gives a list of all past words in ascending order.
 
You can also listen for tweets from [@yourmotherisbot](https://twitter.com/yourmotherisbot). For example, you could wait for it to tweet, then access current.txt for the JSON data. Another option is to use the Discord webhook sent to the [Your Mother Bot Official Server](https://discord.gg/NGKSCxyXtq). There is an announcement channel called #data with a webhook, which you can add to your own server to listen for.

## Format
```
['yyyy-mm-ddThh:mm:ss.zzzzzz+hh:mm', number, 'Your mother is', 'word', 'Pronunciation/Similar to', 'Definition: definintion', 'Synonyms: synonym, synonym']
```

current.txt is in the format `{'data':list}`, while past.txt is in the format `{'data':[list1,list2,...]}`

## Example
View an example of how the data is presented at https://yourmotheris.ajlee.repl.co/ as well as [@yourmotherisbot](https://twitter.com/yourmotherisbot). In addition, join the [Your Mother Bot Official Server](https://discord.gg/NGKSCxyXtq).

## Source code
View the code that maintains this repository at https://github.com/ajlee2006/yourmotheris-code/

## Past runs
22 May 2021 ([previousrun.zip](https://raw.githubusercontent.com/ajlee2006/yourmotheris-data/main/previousrun.zip)): reset the entire system to implement a better past storage system where all past entries are stored in one file, because max 1000 files could be obtained via Github API. The previous system was one text file for each word.

27 Jun 2021 ([previousrun2.txt](https://raw.githubusercontent.com/ajlee2006/yourmotheris-data/main/previousrun2.txt)): 1 MB is the maximum file size obtainable for Github API, so the bot broke and I had to reset it. Previously, it was 10-minutely, and now I have changed it to hourly.
