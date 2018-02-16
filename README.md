# COLLABORATIVE LIBRARY PROTOTYPING

Demo website https://hybrid-publishing-group.github.io/cos-library/

Sample Zotero group https://www.zotero.org/groups/1838445/o-s

Question, need help? See the wiki and issues above on the repository or DM on Twitter https://twitter.com/mrchristian99

# How to make your own collaborative library prototype!

## The Basics

### What you'll get

The following steps will enable you to create a website using Github-pages from a Zotero group. If all goes well you will have a website running in less than 30 minutes. Promise :-)

### Before you start

You will need the following: a Github account; Github access Github Desktop Client or via command line; and a Zotero account.

Create a Github account and download the Github Desktop Client https://github.com/

To use Git via command line, see setup https://help.github.com/articles/set-up-git/

Create a Zotero account https://www.zotero.org/user/register/

The client and browser plugin are not totally necessary but good to have and highly recommended, you will need to authenticate these clients / browser plugins using your account details https://www.zotero.org/download/

### Setup

1. Fork the repository on Github to your user account or organization account. See the 'fork' button top right. https://github.com/TIBHannover/collaborative-library-prototype

2. Now download the repository 'fork' copy to your local machine for editing, see 'Clone or download' button top right of your forked repository.

3. Load your local copy of the 'Collaborative Library Prototype' into your browser. To do this open the index.html file into your browser. You now have the library running locally.

4. Now you need to get access to the Zotero API to be able to add your own content from Zotero groups into your Github-pages website.

You need to have access to a Zotero group, either by being a member of a public group, or by make a new group of your own. See group access and group creation here on the Zotero website, https://www.zotero.org/groups/

Now lets get your API access key. Log into the Zotero website and navigate to https://www.zotero.org/settings/keys . Select 'Create new private key' and make your key. Give it a name; uncheck access to your personal account; check 'Per Group Permissions' and give 'read' access to the group(s) you want to use on your Github-pages website.

Save.

You will be presented with an API key number, copy this and keep it in a text editor. If you need to get hold of your key again you can find it in the address bar on your browser of your 'key edit' page. Example key https://www.zotero.org/settings/keys/edit/mSXXZZUo4xiNPM0tQ0XXXXX

5. Next in Zotero we need to access a 'collection' in a 'group', https://www.zotero.org/groups/ If you don't have a 'collection' already create one online, go to group page and find the 'Group Library' link in your online group and top left you can click the button to add a 'collection'. Once you have chosen your 'collection' navigate to its address online in your group, like so https://www.zotero.org/groups/1838445/o-s/items/collectionKey/BHE6RI6Z

There are two parts that you need from this URL to connect your collection to Github-pages. The group number and the collection key. As you can see from the sample address above these will be 'group=1838445' and 'collection key=BHE6RI6Z'.

6. Now to connect your first 'collection' to Github-pages, you will need your API key, group number and collection key. In your downloaded local repository directory navigate to the HTML file 'os-library.html', open it in a text editor ( like https://atom.io/ ) and go to line 144

`$.getJSON('https://api.zotero.org/groups/1838445/collections/BHE6RI6Z/items?key=mS6PZZUo4xiNPM0tQ0aXXXXX&limit=100&sort=title', function(incomingData)`

Paste in your group number, collection key, and API key like so above. Save the file.

Your locally running website will now be reading the content from your Zotero group's collection. You need to navigate from your home page /index.html to the first collection on your home page /os-library.html, reload this page and you will see the changes. Done!

7. Now to load the repository back into Github and Githib-pages (AKA a push). Go to your Github Desktop client and click on the repository that you want to upload. You will need to add a 'summary' of changes e.g., 'add API details', and then commit and push. Once accepted your files will be synched with GitHub and be available on your Github-pages address, https://username.github.io/collaborative-library-prototype/ where 'username' is your personal user name or Github organisation name.

This is the end of Basics. Your there! This covers Zotero and Github setup, and connecting the two to make your Github website.

Next in 'Finishing up' will be to connect the other sample Zotero collection and how to edit the site and page title, and descriptions in the HTML webpages.

### Finishing up



### How it all works



### Advanced configuration



### More features



### Prototyping




## Tidying up



## How it all works















# Credits and copyright

All content copyright the respective authors and contributors as Creative Commons Attribution-ShareAlike 4.0 International. All code as GNU General Public License version 3 or Open Source Initiative (OSI) https://opensource.org/licenses compliant open license. Graphics and fonts open licensed.

2017-18

Open Science Lab, TIB; Raquel Eulate (CSS).

2016

2015

Originally from a 3rd September 2015 workshop 'Collaborative Libraries, Zotero Co-creation Workshop - Building a Library Reading Room'

**GitHub workshop guide:** https://github.com/consortium/Collaborative-Libraries  

By Loraine Furter and Simon Worthington of Hybrid Publishing Group, taking place at Medialab Prado, Madrid

Thanks to: Dr. Soenke Zehle, Xm:Lab http://www.xmlab.org/about/institute/. Hidden Histories, which will be screen on the digital façade on September 11th 2015, is an activity within the framework of the InVISIBLE and VISIBLE Cities 2015 Open Call of the European Project Connecting Cities Network, curated by Nerea Calvillo. http://medialab-prado.es/article/gestionando-bibliotecas-colaborativas

# Licenses

All software is OSI compliant. Code generated or contributed in the project GNU General Public License version 3.

All content is open licensed [CC BY-SA 4.0 International](LICENSE.md)

All fonts are OSI compliant

All data and metadata is CC 0
