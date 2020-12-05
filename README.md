# Python Text Editor #
##### Text editor created with Python3 and Tkinter for a GUI, with multithreaded features. #####

To run the file, enter the following command into a terminal
>python3 EditorMul.py

### Functions:
#### File Menu:
![File Menu](FileMenu.jpg)

##### New File:
![New File](NewFile.jpg)
`Text.delete(1.0,END)` is used to clear the whole area.

##### Open File:
![Open File](FileOpen.jpg)
![File Opened](FullScreen.jpg)
`askopenfilename` is used to select the file to be opened.

##### Save File:
![Save](FileSave.jpg)

##### Save As:
![Save As](FileSaveAs.jpg)
`asksaveasfilename` is used to select the file in both instances of save.

##### Switch Theme:
![Light Theme](Light.jpg)
![Dark Theme](Dark.jpg)
`Text.config` is used for switching between the themes.

##### Exit:
`askokcancel` is used to confirm from the user whether they want to exit the application and then `destroy()` method is run to destroy the instance and close the application.

#### Edit Menu:
![Edit Menu](EditMenu.jpg)

##### Select All:
![Select All](SelectAll.jpg)
Tkinter events `select(1.0,END)`, cut, copy, paste are used for the Select All, Cut, Copy, Paste functions respectively.

##### Find:
![Find](Find.jpg)
![Find Result](FindResult.jpg)
>def \__find(self,event=None):
>
>>		t1=threading.Thread(target=self.\__finder());
>
>>		t1.start()
>
>>		t1.join()
>
Multithreading has been implemented in find feature.

##### Find and Replace:
![Find](FindandReplace.jpg)
![FindandReplace](FindandReplace2.jpg)
![FindandReplaceResult](FindandReplaceResult.jpg)
>def \__findNReplace(self,event=None):
>
>>t1=threading.Thread(target=self.\__findNReplaceF())
>
>>t1.start()
>
>>t1.join()
>
Multithreading has been implemented to ensure that Find and Replace does not interfere with working of the editor.

##### Clear All:
![Clear](Clear.jpg)

##### Spell Check:
![File Choose](SpellCheckSelectFile.jpg)
![Spell Check](SpellCheck.jpg)
**Note:** Spell Check function works only with .txt files.<br>
>def \__SpellCheck(self,event = None):
>
>>t1=threading.Thread(target=self.\__SpellChecker())
>
>>t1.start()
>
>>t1.join()
>
Multithreading has been implemented in the Spell Check function to work parallelly and not block the working of the editor itself.

#### Help Menu:
![Help Menu](HelpMenu.jpg)

##### Shortcuts:
![Shortcuts](Shortcuts.jpg)
`messagebox.showinfo()` is used to show the list of available shortcuts to the user.
