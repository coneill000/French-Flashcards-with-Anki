# French-Flashcards-with-Anki
A simple program that streamlines the flashcard making process. It takes French audio files with the desired vocabulary and outputs a Google Sheets document that can be downloaded as a csv file to import into the flashcard program [Anki](https://apps.ankiweb.net/). 

## Getting Started
This program was built using [Google Colaboratory](https://colab.research.google.com/). As of right now, this program does depend on functionality found in the Google Colaboratory environment (although it can be modified for more general use). 
### Running this Program
After copying the Google Colab notebook, simply follow the instructions in the notebook and run all of the cells. A few things to consider:
* If you are placing the audio files in your Google Drive, you need to first mount the drive.
* The current program expects to take in mp3 audio files with a title similar to S.mp3, S-13.mp3, etc. This is due to the way the audio files were preprocessed
* On the topic of preprocessing, the audio files should be already separated, with each file containing one word/phrase
* Any audio files that could not be recognized will be placed in the "error" subfolder for manual review. You will also have to manually update the Google Sheets document. 
### Importing into Anki
First, you should manually review the entries to ensure that the recognition was done properly and the English translation is correct. Once everything is checked, save the document as a csv file. Before importing into Anki, move all of the correctly named audio files into Anki's media folder. Also, make sure that the field mapping is done correctly before completing the import. 

## Program Features/Description
This program acts as a way to speed up the flashcard making process. I was motivated to make this after I decided to include audio flashcards for my French learning. However, manually renaming the audio files and creating the cards can be time-consuming. The program uses Google's speech recognizer to recognize the words in the audio files and rename the files accordingly. It also uses Google Translate to add the English translations. It outputs to a Google Sheets document to allow the user to do any manual adjustment. 
