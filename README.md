Droopy: easy file receiving
======
Mini Web server that let others upload files to your computer

#How to use it?
_Note: [A tutorial on how to set up Droopy on Windows](http://www.techkings.org/general-pc-chat/34104-droopy-tutorial.html) was very kindly written by Ronan. The rest of this section focuses on Linux and MacOSX._

Droopy is a command-line program. I'll suppose you’ve downloaded and saved the file in ```~/bin/```. Go to the directory where you want the uploaded files to be stored, for example:

```
mkdir ~/uploads
cd ~/uploads 
```

Then, run droopy. You can give a message and a picture to display:

```
python ~/bin/droopy -m "Hi, it's me Bob. You can send me a file." -p ~/avatar.png
```

And it's up and running on port 8000 of you computer. Check it out at http://localhost:8000, and give your computer's address to your friends.

![ScreenShot](http://stackp.online.fr/wp-content/uploads/droopy-in-terminal.png)

Type ```droopy -h``` to see all options:

```
Usage: droopy [options] [PORT]

Options:
  -h, --help                            show this help message and exit
  -d DIRECTORY, --directory DIRECTORY   set the directory to upload files to
  -m MESSAGE, --message MESSAGE         set the message
  -p PICTURE, --picture PICTURE         set the picture
  --dl                                  provide download links
  --save-config                         save options in a configuration file
  --delete-config                       delete the configuration file and exit
```

#License
Droopy is a free software distributed under the BSD License.

#Feedback and contribution 
I'd love to hear about your experience using droopy. If you have ideas to improve it, please let me know. Pierre — stackp@online.fr.
