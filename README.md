
InstagramSubject
=================

InstaSubject is a command-line application written in Python that scrapes and downloads an instagram user's photos and videos and then analyzes them to determine what subjects the user is interested in. Use to analyze employees before hiring Use responsibly.

<img src="https://cloud.githubusercontent.com/assets/140931/26286476/8232e15e-3e34-11e7-9e1c-9ecda92950e1.gif">

Install
-------
To install:
```bash
$ pip install instagram-scraper
```

To update:
```bash
$ pip install instagram-scraper --upgrade
```
Alternatively, you can clone the project and run the following command to install:
Make sure you cd into the *instagram-scraper-master* folder before performing the command below.
```
$ python setup.py install
```

To analyze images using Amazon Rekognition:
upload images downloaded to S3 bucket
In S3.py, replace name of bucket and replace credentials of AWS

Run
```bash
$ python s3.py
```

Usage
-----

To scrape a user's media:
```bash
$ instagram-scraper <username> -u <your username> -p <your password>             
```
*NOTE: To scrape a private user's media you must be an approved follower.*

*By default, downloaded media will be placed in `<current working directory>/<username>`.*
