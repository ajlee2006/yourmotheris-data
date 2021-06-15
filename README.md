# yourmotheris-data
## UPDATE 22/05/2021
I reset the entire system to implement a better past storage system where all past entries are stored in one file. The previous words are downloadable at [previousrun.zip](https://raw.githubusercontent.com/ajlee2006/yourmotheris-data/main/previousrun.zip) 

## yourmotheris-data
Data for the 10-minutely Your Mother Is word.

## Accessing data
[current.txt](https://raw.githubusercontent.com/ajlee2006/yourmotheris-data/main/current.txt) gives JSON data of the latest word. [past.txt](https://raw.githubusercontent.com/ajlee2006/yourmotheris-data/main/past.txt) gives a list of all past words in ascending order.
 
Alternatively, you can listen for tweets from [@yourmotherisbot](https://twitter.com/yourmotherisbot). For example, you could wait for it to tweet, then access current.txt for the JSON data.

## Format
```
['yyyy-mm-ddThh:mm:ss.zzzzzz+hh:mm', number, 'Your mother is', 'word', 'Pronunciation/Similar to', 'Definition: definintion', 'Synonyms: synonym, synonym']
```

current.txt is in the format `{'data':list}`, while past.txt is in the format `{'data':[list1,list2,...]}`

## Example
View an example of how the data is presented at https://yourmotheris.ajlee.repl.co/ as well as [@yourmotherisbot](https://twitter.com/yourmotherisbot)

## Source code
View the code that maintains this repository at https://github.com/ajlee2006/yourmotheris-code/
