### About PukkaJ-in

PukkaJ-in directory is being listened by the class `backend/PukkaJListener.py` (the listener). 
Every time there are new studies (in the format specified below), the listener will parse the XML files, inference the 
image using PIPNet, and store the results and relevant details in database.
This is a demo directory only. 
### Format: 

Every study placed in the PukkaJ-in directory should be in the following format:

``---StudyUID`` <br>
&nbsp;&nbsp;&nbsp;&nbsp;``|---Image1UID.xml`` <br> 
&nbsp;&nbsp;&nbsp;&nbsp;``|---Image1UID.jpg`` <br>
&nbsp;&nbsp;&nbsp;&nbsp;``|---Image2UID.xml`` <br>
&nbsp;&nbsp;&nbsp;&nbsp;``|---Image2UID.jpg`` <br>

Files without correct formatting will be ignored by the listener, and can cause problems. 