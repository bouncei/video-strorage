# video-strorage
This is a assignment project for internship position in RPAlabs. I have decided to use Flask, Python web framework for this project.


# Requirements

- Python 3.7 or above
- Flask 2.1.3 or above


Required python modules are given in `requirements.txt`.

# Installation

You can install the required modules using 
`python3 -m pip install -r requirements.txt`

Make sure you are using virtual environment if not you can use 
`python3 -m pipenv install -r requirements.txt`
to install the modules in a new virtual env


| Endpoints     | Methods       | Result            |
| ------------- |:-------------:| :----------------:|
| upload/       | POST          | upload video      |
| files/        | GET           | list all videos   |
| charge        | POST          | calculate cost    |
# upload/

The upload api endpoint is to upload and validate and store file in database


# files/

 I integrated a simple query, based on name, max video duration or maximum size (you can perform only one type of query per request)



# charge/ 

The charge api endpoint will take video size, length and type as input, do validation and return charges to the user as applicable.


Charges: 5$ for video below 500MB and 12.5$ above 500MB. Additional 12.5$ if the video is under 6 minutes 18 second and 20$ if above.