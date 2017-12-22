# 100 Days Of Code - Log

### Day 1: December 12, Thursday

**Today's Progress**: I've been working on the Roller Blinds Wifi project, investigating why does my stepper motor (BYJ48) always spin in the same direction using J5. I found that the problem is related to the sequence of the motors, J5 is using a different from the one that specify the builder, [here](http://eeshop.unl.edu/pdf/Stepper+Driver.pdf) is the documentation about it. What I tried:
- Rebuild from scrath the Stepper library using J5.Pin, but for a strange reason that I didn't have much time to see it doesn't like moving the stepper with Arduino's code.
- Create a new issue in J5's repository to see if anyone had this trouble and how I can manage to solve this problem. I looked up in the codebase of the framework but I didn't find anything related to the sequence.

#### Overall status: Good

**Link(s) to work**
1. [Roller Blinds Wifi](https://github.com/EmaSuriano/roller-blinds-wifi)
2. [Issue in J5](https://github.com/rwaldron/johnny-five/issues/1424)

### Day 2: December 13, Wednesday

**Today's Progress**: I've been working with Cato trying to understand J5's code of Stepper class and see how we can change the sequence of the stepper. To do this we clone J5 repo and add a simple test connection file in order to be able to debug it. Sadly, we didn't find anything ... Right now there are 2 reasonable possibilities:
1. Keep looking in the Stepper class code, there are strange variables like `this.io` that I think that has the magic inside.
2. Implement another driver (fisically) that works with 2 pin so we don't have this Direction problem anymore, to do that I have a Pololu driver but it works with 9V so we need a power supply to make it work.

#### Overall status: Bad

**Link(s) to work**
1. [Fork J5 repo](https://github.com/EmaSuriano/johnny-five)

### Day 3: December 14, Thursday

**Today's Progress**: Tired of working with the blinds project I decided to create a new repo in order to test how integration tests could be done. I'm following [this article](https://medium.com/@skidding/testing-react-components-30516bc6a1b3) which at first sight seems really cool. So, I started working on a Weather Application that make a fetch when the component mount on the DOM, dispatch some actions, reducers take that aciton's types and then with some selectors I get the values that will be using my component. The idea is to see how far I can get to test this small application and also, see if give value for the application.

#### Overall status: Good

**Link(s) to work**
1. [Weather app - Integration Cosmos](https://github.com/EmaSuriano/weather-app-integration-test-cosmos)

### Day 4: December 15, Friday

**Today's Progress**: So after having a lot of troubles with CORS calling the weather API of [Open Weather](https://openweathermap.org/ap), I decided to move foward to another onen and it was the best decition I took today. It has the ability to get the forecast with latitude and longitude, which is great because I star the project with that idea. Also I can get many forecast that I want, but I think I'll keep with 6. Next steps are:
* Adding Weather Cards with CSS Grid
* Adding Location Bar
* Add the posibility to refresh the weather
* Finally and the more important is to start making integration testing with cosmos!

#### Overall status: Good

**Link(s) to work**
1. [Weather app - Integration Cosmos](https://github.com/EmaSuriano/weather-app-integration-test-cosmos)
2. [Weather API](https://www.apixu.com/)

### Day 5: December 16, Saturday

**Today's Progress**: I started coding at 3 pm  and finished at 3 am of Sunday, so today was really heavy! The most important thing that I've done was be able to change the sequence when moving steps with the Stepper library of J5, that took almost the whole day ( I had ot fork ConfigurableFirmata repository in order to be able to debug it) but it's working excellent :) Another thing was to advance with the server: 
* It has the possibilty to communicate with socket (using [Socket.IO](https://socket.io))
* It is saving the position on a Local Database (using [NeBD](https://github.com/louischatriot/nedb))

#### Overall status: Good

**Link(s) to work**
1. [Roller Blinds Wifi](https://github.com/EmaSuriano/roller-blinds-wifi)
2. [ConfigurableFirmata](https://github.com/EmaSuriano/ConfigurableFirmata)

### Day 6: December 17, Sunday

**Today's Progress**: I started learning CSS grid to implement it on the weather-react-cosmos app just to give it responsive design. Also made some change sin order to have icons representing the waether, my idea is using icons that have a bit of movement just to make it nicer :) 

#### Overall status: Regular

**Link(s) to work**
1. [Weather app - Integration Cosmos](https://github.com/EmaSuriano/weather-app-integration-test-cosmos)
2. [CSS Grid Garden](http://cssgridgarden.com/)
3. [CSS Grid Tricks](https://css-tricks.com/snippets/css/complete-guide-grid/)

### Day 7: December 18, Monday

**Today's Progress**: I worked on impementing enviroment variables on roller-blinds-server and also adding async/await in order to avoid using promises. Also, I made the first iteration to integrate Redux with Socket.IO and work very well there are some issues and error handling that I have to take care of but fortunatetly the socket itself is working for more than one client.

#### Overall status: Good

**Link(s) to work**
1. [Roller Blinds Wifi](https://github.com/EmaSuriano/roller-blinds-wifi)
2. [Redux Socket IO](https://github.com/itaylor/redux-socket.io)

### Day 8: December 19, Tuesday

**Today's Progress**: I added error handling on the server side (it will return an action with the type 'SERVER_ERROR' with the message), then on the client I added a notification system so when it received an errror it will show a notification on the left bottom corner.

#### Overall status: Good

**Link(s) to work**
1. [Roller Blinds Wifi](https://github.com/EmaSuriano/roller-blinds-wifi)
2. [React notification](https://github.com/pburtchaell/react-notification)

### Day 9: December 20, Wednesday

**Today's Progress**: With the team we did the integration of the apps with the roller blinds server. It's working pretty well but we're having some troubles connecting to the server from our client (Marcos computer).

#### Overall status: Good

**Link(s) to work**
1. [Roller Blinds Wifi](https://github.com/EmaSuriano/roller-blinds-wifi)


### Day 10: December 21, Thursday

**Today's Progress**: We add validation to the roller blinds in order to prevent from moving if the server doesn't respond with a succesfull response. After doing this, we kind of broke the whole server/application and also there are some strang behaviour inside the server. Besides that, we did the presentation talking about the scope of the project, architechture and communication between all the parts of it. 

#### Overall status: Regular

**Link(s) to work**
1. [Roller Blinds Wifi](https://github.com/EmaSuriano/roller-blinds-wifi)
