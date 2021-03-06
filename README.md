Natural Order Japanese
======================
![Screenshot of lookup feature](https://cloud.githubusercontent.com/assets/1934920/4873818/1c72537c-6227-11e4-893d-d2117fa18b0a.png)
If you're learning Japanese, you might have come across the infamous Sentence Mining approach. 
This involves collecting and reviewing thousands of example sentences in a flashcard/SRS program.
Where are you going to get these example sentences?
What if these example sentences are too easy/hard for you?

Natural Order Japanese is a cross-platform electronic dictionary focused on example sentences. 
You can import dictionaries like EDICT and Daijirin so that all your example sentences are in one place.
You can also import your Anki flashcard deck. This means the program can determine what vocabulary you 
already know and give difficulty scores to the example sentences relative to your knowledge.
All that's needed to get example sentences is to do a single lookup of a word you want to learn.
This makes sentence mining a much more efficient process, meaning you have more time to learn and enjoy the language.

Compiling
---------
 - Install [MeCab](https://code.google.com/p/mecab/) and the Python binding ([MeCab installation guide](https://github.com/mcho421/noj/blob/master/installing-mecab-python.md))
 - Install [Qt4](http://qt-project.org/) and [PyQt4](http://www.riverbankcomputing.com/software/pyqt/intro) ([PyQt4 installation guide](http://www.pythoncentral.io/install-pyside-pyqt-on-windows-mac-linux/))
 - Install Python libraries with ```sudo pip install -r requirements.txt```
 - Compile resources with ```./make_resources.sh```
 - Run ```python noj/__init__.py```
 - If you would like the JMDict/EDICT dictionary: 
   - [Download the database](   https://drive.google.com/file/d/0BxolPhoJ07QdY0tDT0ltckRyM00/view?usp=sharing) 
   - Move `database.db` to `~/Documents/Natural Order Japanese`

TODO
----
The Anki importing isn't available on the GUI yet. For the time being, you can do the following:
 - Edit ```noj/importers/anki_importer.py``` with your Anki Deck settings
 - Run `python noj/importers/anki_importer.py`

See the following projects for importing additional Sentence Libraries:
 - https://github.com/mcho421/noj_dumpers
 - https://github.com/mcho421/noj_converters

Licence
-------
[GNU General Public Licence v3](http://www.gnu.org/copyleft/gpl.html)

Contributors
------------
[Mathew Chong](https://github.com/mcho421) (mathewchong.dev@gmail.com)
