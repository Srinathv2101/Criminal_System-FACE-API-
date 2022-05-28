# CRIMINAL SYSTEM
This script makes use of Python, Flask and Microsoft Azure FaceAPI for face detection, personGroup creation/deletion and Person-To-Face comparision. 

## Steps
1. Install the python libraries using pip:
<pre>
pip install -r requirements.txt
</pre>

2. Give permissions to the scripts for Linux(not necessary for Windows):
<pre>
chmod +x create_person.py
chmod +x find_person.py
</pre>

3. Obtain a Microsoft Azure FaceAPI Endpoint and Key. Place both in the setup.py file. The API subscription used is Free Trial and Pricing tier is standard S0(10 api calls per second). The free F0(20 api calls per minute) pricing tier also works aslong as the api calls made are less than the limit. 
Link: https://azure.microsoft.com/en-us/services/cognitive-services/face/
 

### Many-To-One
Description:  Given multiple image files and a specific target(criminal already present in database), will display all the image files with specified target in it.
<pre>
python find_person.py
</pre>

### One-To-Many
Description: Given a single image, system will return the image with boxes marking the heads of all criminals present in it.
<pre>
python find_person.py
</pre>

## Operating Systems
This script is supported on Windows, Linux, and MacOS.

## How-To Video
[![How To Video]](youtube_url)
