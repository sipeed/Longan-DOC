Longan board
==========

Wiki for Sipeed Longan series boards. 



|[Read me online](https://longan.sipeed.com/en/)  | [在线阅读](https://longan.sipeed.com/zh/) |
| ------------------------ | ----------- |

[![Build Status](https://travis-ci.org/sipeed/Longan-DOC.svg?branch=master)](https://travis-ci.org/sipeed/Longan-DOC)





## Build Doc


This documentation site is powered by GitBook. You can check out the online version here.

You need Node.js and npm to be able to build the site.

To install gitbook:

```
npm install gitbook-cli -g
```

Get Doc source code:
```
sudo apt install git 
git clone https://github.com/sipeed/Longan-DOC.git
```

Install gitbook plugins:

```
cd Longan-DOC
gitbook install
```

Serve as a website:

```
chmod +x serve.sh
./serve.sh
```

Then visit http://localhost:4000


