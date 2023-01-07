# Digital-logic-design-pong-game-in-verilog
The game presented is a single-player implementation of the classic sport Ping Pong. With respect to the salient
features of the presented project, there is a implementation of a counter which serves as a score mechanism.
The score is incremented with each successive hit off the player’s paddle while the score is reset following the
player’s failure to make contact with the ball object. The main objective of the game is for the player to achieve a
high of a score that is possible - the game ends when the player achieves a specific score.
![dsfsdfsd](https://user-images.githubusercontent.com/62338143/211174528-8485e8db-9615-44a4-8499-2e73f8ac9240.png)



# Finite state machine 
![fsm](https://user-images.githubusercontent.com/62338143/211174416-d2e1859b-457d-4dbd-b756-079f77633492.png)


# Results
In our VGA module we have successfully shown that the ball changes both its speed and direction when it
collides with either the walls or the paddle. This can also be seen in Figure 20. Accordingly, if the ball successfully
bounces off the paddle, the current score of the Player increments by an seed of 1 (as shown in our Scoring
module). However, if the Player is unsuccessful in making contact, the score is reset back to 0 and thus, loses
the game. We have implemented our major state transitions using the Major FSM while the Collision state
contains Minor FSM in order to simplify the functionality of the state transition system. In this way, we have used
the Major-Minor FSM system.
The FSM is modeled as a Circular FSM - at every positive edge of clock cycle there will be a state transition.
These transitions would occur rapidly thus, keeping the illusion of a simultaneous execution of sorts.


![sdsds](https://user-images.githubusercontent.com/62338143/211174412-06f7db74-d9be-4ebe-9c19-226c1b7a33f6.png)
