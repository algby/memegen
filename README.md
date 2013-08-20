memegen
=======

In House Meme Generator

This is designed to be drop and use as much as possible.  Designed for office use to create memes to be used for in office chat.

To Run:
```bash
python flaskr.py
```

Features
========
* New Image Template Upload
* Creates static links for all memes generated

How It Works
============

Memegen stores all images on the local file system in the static/images and static/memes folders.  memegen.db is a sqlite3 database that keeps track of all the files in these folders.

Memegen uses PIL (Python Image Library) to write text on images.

Very little work needs to be done to serve this application on httpd, lighthttpd, or nginx.  However due to load requirements there is little need as no more then a handful of people will ever be using it at once.

Requirements
============
* flask
* PIL
* sqlite3
