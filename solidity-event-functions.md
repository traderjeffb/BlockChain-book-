# Event Functions

##### By using events you can access the EVM logging faciilties  which you can then use for JavaScript "callbacks" -this will allow you to listen to the events.

it's best explained though an example.

Copy the code below into Remix:

```
pragma solidity ^0.4.21;

 contract homeRoomTeacher {

     string firstName;
     string lastName;
     uint homeRoomNum;
     address owner; 

     event homeRoomTeacherEv(
        string firstName,
        string lastName,
        uint homeRoomNum
         );

    function homeRoomTeacher() public{
        owner = msg.sender;
    }

     function setHomeRoomTeacher(string _firstName, string _lastName, uint _room) public {

         firstName = _firstName;
         lastName = _lastName;
         homeRoomNum = _room;
        homeRoomTeacherEv(_firstName, _lastName, _room);
     }

     function getHomeRoomTeacher() view public returns ( string, string, uint){
         return ( firstName, lastName, homeRoomNum);
     }
 }
```

Above you will see that we our homeRoomTeacher contract with 3 variables- firstName, lastName and homeRoomNum. Below that we have created a event function that will emit any time someone changes the values of our home homeRoomTeacher. Below that we have the function setting the owner. The bottom 2 functions are setHomeRoomTeacher and getHomeRoomTeacher. 



Anytime we call our setHomeRoomTeacher function we are going to to emit a homeRoomTeacherEV event. We can see this event happen in the bottom terminal window. Let's try it now. On the right in the tabs panel you should have 2 boxes a blue setHomeRoomTeacher and a getHomeRoomTeacher. In the text box to the right of setHomeRoomTeacher you will notice it tells you exactly what it needs - a string, a string and a uint.



 In the text box enter a first name, last name & a room number each one in quotes and separate by commas. Once this is complete click the red button to set the information you just entered. Now, click the blue button to get the information you just entered. 

