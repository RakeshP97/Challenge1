# Challenge:
Loading Largest File into DB

Prerequisites to run Jar:

Need to download the winutils.exe and placed it inside the C:\winutils\bin folder.
Mango DB need to install before running this Jar.
Java Code Details: class name: LoadFile.class Main(): Load the custom file and create the spark Objects and call the list of methods to perform some set of operations on the RDD. calculateWordMap(): This method will do parsing rdd and calculated the word count return the hashmap contains word as key and value is count. sortedWords(): Words going to sort based on the count values by using custom comparator logic.

reverseSortedWords(): Words going to sort in reverse order based on the count values by using custom comparator logic.

insertIntoDB(): Taking parameters as hostname and portnumber as an CL argument and connected to Mango DB to insert document records for the each word with count value.

displayEntries(): Taking parameters as hostname and portnumber as an CL argument and connected to Mango DB to retrieve the documents from the DB.

To Execute the Jar File: java –Xmx8192m -jar challenge.jar –source C:\MyData\enwiki-latest-pages-articles-multistream-index3.txt –mongo localhost:27017
