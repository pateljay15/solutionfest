# solutionfest
Demo purpose the live link of application:
-> https://ngo-helpers.netlify.app/

Dummy Normal IDs:
email: user@gmail.com
pass: user@123

Dummy NGO IDs:
email: ngo@gmail.com
pass: ngo@1234

NOTE::::  For better experience of receiving real time mails plz use 
your real emails IDs to register in this application.

Also we haven't deploy the code to the server which send realtime notifications to  ngos about nearby 
places which needs to be cleaned and maintain well via email 
bcoz it will charge us as we are using AWS for sending emails. 
But you can see the code for the same in : 
backend/controllers/realTimeNotify.js

Tools used:
Backend: Nodejs , Express
Frontend: ReactJS
Database: MongoDB

prerequistic for running this application:
your computer has nodejs latest version installed and also react

Set up Frontend:

1) cd frontend/client
2) npm install
3) npm start

setup for backend:

1) cd backend
2) npm install
3) node index.js



### Problem statement:
There are many places where animals and birds are found earlier but because of increase in the waste and lack of cleanliness and increased use of plastic , animals are suffering
from various diseases and are becoming extinct day by day. And sometimes  NGOs who work for animal welfare are unaware of such places in the city . So the solution which we have
proposed will be aiming to create a network of NGOs and citizens of the city to work together to identify those places and make the nearby NGOs aware about those places to make
that place better again which is suitable for the living habitat of that area.

###  Important feature which we are talking about is:

The code for this is in backend/controllers/realTimeNotify.js

This system will peridocally checks the database and will iterate over all places which needs to be cleaned and all ngos registered with the system and will check
all ngos whuch are nearby the places which need to be restore based on the condition like similar mathching pincode, noOFPeople needed to restore that place is less than
the noOFActiveMemebrs of the ngo and then this system will automatically send email to all the nearby NGOs informing about the place which they should look for
in order to restore that place



