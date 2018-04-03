- How to Run -
My visualization is implemented through the Python file fileReader.py. This uses a flask implementation, and so must be run from the command line. After which, the visualization can be viewed from the link below:



http://127.0.0.1:5000/run/3/



The final number (3 in this case) represents how the maximum grade level kanji would be represented in the visualization. This number can be changed to any integer between 1 and 11, though it is recommended to limit the number to 6 or 7 at most, otherwise the visualization becomes far too convoluted.



- Files included
data_changes.txt: Describes the edits made to the datasets


dataTrimmer.py: A script used to trim the full dictionary down to a manageable size


fileReader.py: The main script used to parse the data into the JavaScript through 
flask

kanjidic2.xml: The original JMdict database containing detailed kanji descriptions.

kanjitrim.txt: The kanjidic2 database parsed into just the kanji and the grade in which it is taught
kradfile#(1-11): The KANJIDIC2 database with any kanji taught in a grade greater than # is removed


kradfileFull: The original KANJIDIC2 database


Report.pdf: The PDF write-up describing my visualization


static/kanji.js: The JavaScript file that deals with the bulk of the actual visualization using D3


templates/kanji.html: A go-between that passes data from fileReader.py to kanji.js, and also calls kanji.js.
