https://ubuntuhandbook.org/index.php/2021/01/install-linux-mints-web-app-manager-ubuntu-20-04/

Download File from and save: 
http://packages.linuxmint.com/pool/main/w/webapp-manager/webapp-manager_1.1.9_all.deb

```
sudo apt install ./Downloads/webapp-manager*.deb
```

Download File from and save: 
http://packages.linuxmint.com/pool/main/l/linuxmint-keyring/linuxmint-keyring_2016.05.26_all.deb
```
sudo apt install ./Downloads/linuxmint-keyring*.deb
```

Es wird im Terminal angegeben, das dies nicht als Root durchführbar wäre, funktioniert aber trozdem.

Im `Startmenü` unter `Internet` wird `Webapps` aufgelistet, von dort ausführen. 

# Webapp Manager

Run websites as if they were apps.

FAQ
===

How to go back without the navigation buttons?
----------------------------------------------

Right-click an empty area of the Web page to show the context menu. In most browsers this menu contains navigation buttons.

How to open links in my main browser?
-------------------------------------

For Firefox, all links are always opened within the WebApp, either directly or using a new tab.
To open a link in your main browser, right-click anywhere, select `Copy link location` and paste the link in your main browser. 

Chromium and Chrome WebApps open external links in the main browser.

How to use tabs in Firefox?
---------------------------

Press `Ctrl`+`Tab` to cycle between opened tabs.

Press `Ctrl`+`T` to create a new tab.

Press `Ctrl`+`W` to close the current tab.

Press `Ctrl` when clicking a link to open it in a new tab.

How to add extensions in Firefox (AdBlock etc.)?
------------------------------------------------

Press and release the `Alt` key to show the main menubar.

You can then reach the `Add-Ons` from the `Tool` menu.

How to add extensions in Chromium based browsers (AdBlock etc.)?
----------------------------------------------------------------

Press `ctrl+N` to open a new window.

Navigate to https://chrome.google.com/webstore/category/extensions

Now add the extension.




## How to Remove Web App Manager:

To remove the application, simply open terminal and run command:
```
sudo apt remove --auto-remove webapp-manager
```
To remove the Linux Mint repository, remove the relevant line from Software & Updates -> Other Software.

And you may also remove the config file created to set the priority, via command:
```
sudo rm /etc/apt/preferences.d/mint-ulyssa-pin
```

Hierbei wird `Webapps` aus dem Verzeichnis `Internet` im `Startmenü` wieder entfernt. 
