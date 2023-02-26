# ChatGPT
A small desktop application to interact with ChatGBT 

Requirements will be added here as we go along the development process. 


Firstly Requirement of a Python IDE, I will be using Pycharm in this build.


Python Dependancies will grow so they will be added here for ease of use, but the Git file should contain all required dependancies


https://git-scm.com/download/win


Will require Requests Libary inside Python :

pip install requests

Current Build 2023/02/26 15:00 Update 

Userform is using the incorrect API location and command might need to look at another method Potentially looking at openai Library 
https://platform.openai.com/docs/api-reference/authentication

API call is redundent in current build but I want the API connection to be a serperate entity from the Userform application due to API keys and active sessions being differnet ( Application would crash if two GET requests are sent using the same token from different IP's??) 

API testing is a stand alone Module that just sends a HTTP request to https://api.openai.com/v1/completions" 

changes need to be made to data fields below for different results

data = {
    "model": "text-davinci-002",
    "prompt": "What model is this?",
    "temperature": 0,
    "max_tokens": 50
}


Example Change "prompt" value (Change string value of parameter <"What model is this?"> ) if you want different answers

The response of this script is currently just being printed in the run window within Pycharm see Example A .jpg as reference





