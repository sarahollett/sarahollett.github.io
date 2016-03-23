#Intro to the Zotero API

First need to download libZotero, a Python module that allows you to interact with Zotero API, with`pip install libZotero`

From here, we can follow each step, but when we reached `for item in items: print item.bibContent` to get full bibliographic information we received an error that read:

![unicode error](http://s29.postimg.org/cj0pc6hyf/unicodeerror.jpg)

After you follow the instructions for getting Unicode, start back at the beginning. After `from libZotero import zotero`, then tell Python the user/group code and API Key for the Zotero library you want to use.

If we use the Programming Historian Library they advise, we get no input with the command, `items = zlib.fetchItemsTop({'limit': 5, 'content': 'json,bib,coins'})` 

As well as we don't get the same metadata detail from command, `for item in items:
print 'Item Type: %s | Key: %s | Title: %s' % (item.itemType,item.itemKey, item.title)`

![Programming Historian Zotero Library](http://s29.postimg.org/biiu60uhz/proghistzoterolib.jpg)

However, by synching the information we inputted into Zotero Standalone Desktop in the Pandoc Tutorial we can request the Zotero API to provide our own metadata. To synch, go to Actions>Preferences>Sync and enter our account information.

![synching account](http://s9.postimg.org/5cfpz3ldb/zoterosynch.jpg)

The information you inputted into the desktop are now found online. From here, you need to find your User code and API Key to tell Python where your account API is located. To do this, go to Settings>Feeds/API. Your userID will be displayed and from there you can create a 'new private key'.

![Zotero account API/userkey](http://s10.postimg.org/byjtybr55/Zotero_API.jpg)

Now you can replace `zlib=zotero.Library('group','155975','<null>','9GLmvmZ1K1qGAz9QWcdlyf6L')` with your information, switching `group` with `user` and inputting your own user code and API Key.

![personal library results](http://s10.postimg.org/4jz3jound/personallibrary.jpg)

This is an interesting way to see the organization of your own metadata or if you wanted to pull sources from a group's or person's Zotero account. However, I wasn't sure if you could just look up the API keys for groups or if you needed to be a member. For example, I wasn't able to find the information they provided in the tutorial (user code and API key) on the Zotero account of Programming Historian example. 

Tutorial 2: Creating a New Item

Simple to follow instructions and easy to follow directory at the end so you can add various types of entries (document, videos, etc). But I received `403: Write access denied` when I inputted commands and ran the commands as a script. 

![Creating New Item error](http://s13.postimg.org/u4ugxd5nb/creatingnewitem.png)

![Creating New Item with script](http://s21.postimg.org/rgh4hcrh3/createnewitemwithscript.png)

