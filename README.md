# MessagingApp

This app is a one to one messaging app made using android studio and coupled with firebase firestore.
Andriod devices with API above 25 are prefered //I have used pixel 2 API R
This app uses Email Password Authentication.
I do recognize the requirment of phone number verification using OTP, which is possible using firebase services but to prevent complexity I have assumed that the phone number added are unique for each email( also it prevents us from using emulator)
You donot need to signin each time, the login activity will redirect you to dashboard automatically unless you sign out
To send a message to another user it is compulsory for you to have him in your contact list
messages sent by other users wont be visible to you untill they are in your contact list, though you can view the previous messages once u add them to your list
My database consist of three collection:
1) UID:  this collection consists of a map between Each UserID and their phone number.
2) Messages:it consists of documents which contain the chats. A new document is created each time a new  unordered contact pair is added
   this design also makes it easy to adapt this app for group chats.
3) users: it consists of the list of contacts of each user

All the data is stored at the backend hence internet connection is must
to run this app on your emulator & to have a look at the database behavior and structure U will need to connect it to fireStore database(you may also need to instantiate the collection names)
I am also providing a snapshots of the database
