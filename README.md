# ACC-SKYSCANNER


Web Crawler
* A web crawler, also known as a crawler or web
spider, is a computer software used to
automatically search and index the content of
websites and other online data.
* Crawlers visit websites in a systematic way to
discover the content of each page so that it can be
recorded, updated, and retrieved in response to a
user's search query.
* After starting with a known set of pages, web
crawlers move on to new pages by visiting on links
from the previously crawled ones.



Data Validation
* Data Validation is performed by using various
necessary regex expressions for obtaining valid
inputs. For eg: Validation is checked for whether a
string is alphanumeric or not.


crawlUrls()
* The method takes input parameters of level, the url link and visited url.
* The method starts the crawling process for the input url and checks whether the url is
visited or not.

crawl()
* The method takes input parameters of level, the next url link and visited url.
* The method checks the level of depth for the input url and starts crawling that url link if it is
not present in the arraylist.

request()
* The method takes input parameters of the next url link and visited url by parsing it.
* The method launches a web browser with the provided url using selenium and extracts the
data from that url.


Data Validation using Regular Expressions
* Regex patterns are used in the above methods to get the necessary and valid data from the
websites

Inverted Indexing
* This can be visualised as an index data structure
that stores a mapping between content—such as
words or numbers—and their frequencies in a
collection of documents.

* We can conduct speedy searches without having to
browse through all of the files because of inverted
indexing.
* The frequency count feature displays to the user
the number of times a word appears in a given url
* Trie is used for storing the words and list of
occurrence of that word in each file


Frequency Count
* It is the process of calculating the total occurrence
of a word in a specific file.
* Hashmap is used for storing the list of words and
frequency of the words.

Inverted Indexing
constructTrie()
* Haspmap is used for storing frequency and filename of word where the key is the
filename and value is the frequency.
* Words and the list of their occurrences in each file is stored using Trie to form an
inverted index.

Frequency Count
hashTable()
* For a given file, the list of words and their frequencies are computed and returned as
output


HTML Parser

* The HTML source data can be transformed using an
HTML parser into a text file, making it simple to
conduct operations on that data.
* Data from HTML parsers also helps in removing
useless data that web crawlers download.
* Java's Jsoup library is used for parsing HTML files

Page Ranking
* Based on the frequency of occurrences, page
ranking is used to evaluate the value of a search
result.
* A website will score higher for search terms that are
used more frequently across the page.
* Hashtable is used for storing the url link and the
frequency count of the words.


HTML Parser

htmlParse()
* Parses the html data from the url into text file using Jsoup.

// FUNCTIONS USED IN THE PAGE RANKING ALOGRITHM
readFile()
* The method is used to read files using Jsoup.

matchPattern()
* Word is taken as input and occurrence of that word is computed in the file.
* Frequency of word is calculated for list of files.
* Hashtable is used for storing and the url link and the frequency of the word where
key is the url link and value is the frequency of word.


Spell Checker
* The spell checker is used for checking the spellings
of the corresponding words.
* It suggests the user a list of alternative words if the
spelling of the input word is incorrect.
* Edit distance algorithm is used for searching
alternative words having minimum edit distance.

Spell Checking
minDistance()
* The method uses the edit distance algorithm with the given input word and the word
with minimum edit distance.

Word Completion
* Word Completion is used for completion of
incomplete words.
* Trie is used for storing the words into a dictionary
from the list of web pages.
* If the word is incomplete, then the word with similar
prefix from the dictionary is returned as output.

Search Frequency
* A word is taken as an input and stored in a file for
calculating the search frequency of that word.
* If the word is found in the hashmap, then the
frequency count of that word is incremented by 1.
* Hashmap is used for calculating the frequency of
the word from the file.

Word Completion
* The List of web pages are read and their words are stored in a dictionary using trie.
* A word is taken as input from the user.
* If the word is incomplete then the words from dictionary with similar prefix are
returned as output.

keysWithPrefix()
* For words with similar prefix the method t.keysWithPrefix() method is used.

Search Frequency
* For search frequency whenever a word is taken as input it is stored in a file named
as search_frequency,txt.
* Using this file the frequency of searched words is calculated and returned as output.
* HashMap is used to calculate the frequency of the word from the file
