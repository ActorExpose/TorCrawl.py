<!--
  Title: TorCrawl.py - GUI Branch
  Description: a python script with graphical user interface based on Gooey to crawl and extract (regular or onion) webpages through TOR network. 
  Author: MikeMeliz
  -->
# TorCrawl.py - GUI /w [Gooey](https://github.com/chriskiehl/Gooey)

[![Version](https://img.shields.io/badge/version-0.6-orange.svg?style=plastic)]() [![license](https://img.shields.io/github/license/MikeMeliz/TorCrawl.py.svg?style=plastic)]()

## Basic Information:
TorCrawl.py is a python script to crawl and extract (regular or onion) webpages through TOR network. 

- **Warning:** Crawling is not illegal, but violating copyright is. It’s always best to double check a website’s T&C before crawling them. Some websites set up what’s called robots.txt to tell crawlers not to visit those pages. This crawler will allow you to go around this, but we always recommend respecting robots.txt.
- **Keep in mind:** Extracting and crawling through TOR network take some time. That's normal behaviour; you can find more information [here](https://www.torproject.org/docs/faq.html.en#WhySlow). 

<p align="center"><img src ="https://media.giphy.com/media/RmfzOLuCJTApa/giphy.gif"></p>

## Installation:
To install this beta branch, you need to clone that repository:

`git clone -b guidev https://github.com/MikeMeliz/TorCrawl.py.git`

You'll also need Socks, BeautifulSoup, [Gooey](https://github.com/chriskiehl/Gooey):

`pip install socks beautifulsoup Gooey`

**Note:** Python 2 users must manually install WxPython! Please, check [wxPython website](http://www.wxpython.org/download.php).
```
pip install -U \
    -f https://extras.wxpython.org/wxPython4/extras/linux/gtk3/ubuntu-16.04 \
    wxPython
```

Of course, the TOR Hidden Service is needed:

Debian/Ubuntu: `apt-get install tor`
[(for more distros and instructions)](https://www.torproject.org/docs/)

## Arguments:
arg | Long | Description
----|------|------------
**General**: | |
-h  |--help| Help
-v  |--verbose| Show more informations about the progress 
-u  |--url *.onion| URL of Webpage to crawl or extract
-w  |--without| Without the use of Relay TOR
-f  |--folder| The directory which will contain the generated files ([@guyo13](https://www.github.com/guyo13))
**Extract**: | | 
-e  |--extract| Extract page's code to terminal or file. (Default: Terminal)
-i  |--input filename| Input file with URL(s) (seperated by line)
-o  |--output [filename]| Output page(s) to file(s) (for one page)
**Crawl**: | |
-c  |--crawl| Crawl website (Default output on /links.txt)
-d  |--cdepth| Set depth of crawl's travel (Default: 1)
-p  |--pause| The length of time the crawler will pause (Default: 0)
-l  |--log| A save log will let you see which URLs were visited

## Demo:
![default](https://user-images.githubusercontent.com/9204902/49688368-7c1f9980-fb19-11e8-851a-5c72ea916d42.png)


## Contributors:
This is a beta version with graphical user interface, please consider the contribution into master brnach, but still feel free on this too! Just fork it, make any change on your fork and add a pull request on current branch! Any advice, help or questions will be great for me :)

## License:
“GPL” stands for “General Public License”. Using the GNU GPL will require that all the released improved versions be free software. [source & more](https://www.gnu.org/licenses/gpl-faq.html)
