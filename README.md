Kadenze-dl
===

Small application to download Kadenze (https://www.kadenze.com) videos for courses you enrolled in.

It scrapes the site content based on your profile information given in the configuration file to download H264 720p videos courses.

I made it in order to have offline access to this great online course : (https://www.kadenze.com/courses/creative-applications-of-deep-learning-with-tensorflow/info), check it out !


Install
---

For now, download and unzip package. Will be on PyPI soon.

Install requirements :
  
    pip install -r requirements.txt

Usage 
---

Replace placeholder fields in the configuration file in YAML format, example :

	kadenze:
    	login: "myemail@gmail.com"
    	password: "mypassword"
	download:
    	path: "/data/kadenze-dl"
    	courses: "course-1"
    			 - "course-2"
    			 - "course-3"


Run the application :

	python kadenze-dl.py