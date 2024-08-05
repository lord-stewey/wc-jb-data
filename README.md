# How to import jumpbridges into EveEye.com

## Why did I do this

I wanted to use EveEye and SMT with our Eve Online alliance jumpbridges and I was struggling to figure out how. Too many dead ends that didn't work. I figured I would share what I did and would love to get some feedback on other ways.

This solition will leverage the use of an extension someone wrote that copies the HTML table on DOTLAN into the clipboard. Then a text editor will be used (I used Notepad++) to format and save the data in CSV format. Finally, EveEye and SMT can then point to the file and import the data.

**NOTE:the data pasted into the text editor had a problem not parsing systems that ended in a 0 (zero). You will want to scan the data from top to bottom and manually fix any defects before saving it.**<br/><br/>

## Chrome Extension

I found this extension and enabled it. Please do your due diligence before installing extensions.

Go to the [Google Store](https://chrome.google.com/webstore/category/extensions) in Microsoft Edge and search for `Dotlan Export Network` then install it.

![Get Extension](images/Screenshot%20-%20search%20extension.png)<br/><br/>

Enable the extension.

![Extention Button](images/Screenshot%20-%20extension%20button.png)<br/><br/>

## Get The Data

You will use the extension on the Bridges page in DOTLAN.

Go to DOTLAN https://evemaps.dotlan.net/ and log in with an account in the alliance you want the jumpbridges for. Requires registration.

![Home Page](images/Screenshot%20-%20navigation.png)<br/><br/>

Click `Navigation` button at the top. Then choose `Bridges`.

![Bridges](images/Screenshot%20-%20bridges.png)<br/><br/>

Choose the `Network Name`.

![Network Name](images/Screenshot%20-%20network%20name.png)<br/><br/>

Next to `Jump Bridge Network: <network name>` hover the mouse to the right of this text and a button labeled `Copy Network` should appear then click it.

![Hover for the button](images/Screenshot%20-%20hover.png)<br/><br/>

![Copied to clipboard](images/Screenshot%20-%20copied%20to%20clipboard.png)<br/><br/>

## Format The Data

You will paste the clipboard you copied from DOTLAN into any notepad like editor to create a .csv formatted file.<br/><br/>

Paste into your favorite text editor.

![Paste clipboard into editor](images/Screenshot%20-%20paste%20clipboard.png)<br/><br/>

Remove everything except the two system names on each row with a tab between.

![Data Format Example](images/Screenshot%20-%20data%20format%20example.png)<br/><br/>

Save the file in a publicly accesible location like github or cloud as a `.csv` file then get a url to the direct file.

## Import The Data

Open [EveEye](https://eveeye.com) and select the `Custom Data` button on the left. Click `jumpbridges` and paste the link into the `External Data` then click the `refresh` button.

![EveEye](images/Screenshot%20-%20eve%20eye.png)<br/>
