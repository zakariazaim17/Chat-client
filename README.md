
# Chat-Client
This application is used for chat messaging.
Implemented features:
+ Multiple users can connect to the application and using it simultaneously : so when a new user uses the application in the back
ground, there is a connection request sent that leads to starting a thread for that connection.

+ The user can log in to the application by a unique username that can't be used by others in case the first user doesn't log out from 
the application.

+ After login the user can send messages as abroadcast to all the other users and the messasge is displayed as form of 
" 'content' from 'username' on 'date' " where the content is the message typed, the username is users nickname by which he loged in and date
is the curremt date when the message is sent.

+ By clicking  ' Messages ' in the menu, the user can access the chathistory of the application that includes all the messages sent from
 every user.

+ By clicking 'Users' the user can see all the usernames that loged in to the application.

+ By clicking  'update' we have three cases for: if the user is in the messages activity he  can eventually see  updated messages 
from others, also if the user is working in the Users avtivity he can see if someone has loged in at that time, and in case the user is
working in the Topchatter activity he can see the updated top chatters at any time.

+ The user can see the top chatters on the application, and chatters are determined by the  number of messages sent during  their activity.

+ the user can log out from the application so his username is deleted from the users list and can be used again by other user. 

....
design patterns used in the client application:
 
 + I used singleton : ClientConnector
 + I  used observer  : ChatClientObserver
 + I used observable : ChatClientObservable
