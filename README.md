# Python Text Editor #
##### Text editor created with Python3 and Tkinter for a GUI, with multithreaded features. #####

To run the file, enter the following command into a terminal
>python3 EditorMul.py

### Functions:
#### File Menu:
![File Menu](FileMenu.jpg)

##### New File:
![New File](NewFile.jpg)

##### Open File:
![Open File](FileOpen.jpg)
![File Opened](FullScreen.jpg)

##### Save File:
![Save](FileSave.jpg)

##### Save As:
![Save As](FileSaveAs.jpg)

##### Switch Theme:
![Light Theme](Light.jpg)
![Dark Theme](Dark.jpg)

#### Edit Menu:
![Edit Menu](EditMenu.jpg)

##### Select All:
![Select All](SelectAll.jpg)

##### Find:
![Find](Find.jpg)
![Find Result](FindResult.jpg)

##### Find and Replace:
![Find](FindandReplace.jpg)
![FindandReplace](FindandReplace2.jpg)
![FindandReplaceResult](FindandReplaceResult.jpg)

##### Clear All:
![Clear](Clear.jpg)

##### Spell Check:
![File Choose](SpellCheckSelectFile.jpg)
![Spell Check](SpellCheck.jpg)
**Note:** Spell Check function works only with .txt files.
> def __SpellCheck(self,event = None):
>		t1=threading.Thread(target=self.__SpellChecker())
>		t1.start()
>		t1.join()
