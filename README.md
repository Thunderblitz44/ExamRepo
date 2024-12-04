# ExamRepo
 
Explanation for what was implemented

-Player inputs
-Attempted to implement command pattern, failed due to the fact I could not use my gdw assignment containing my command design pattern.
Failed to remember a majority of the implementation, created objects for different player inputs but failed to recreate the execution functionality properly. Each command object was supposed to contain an amount to rotate the block but, I failed to remember how to implement the commands being executed and returning their information.
-Implemented game instance singleton so the hud and player script can talk to each other while also being decoupled. Both the player and hud send themselves to the singleton, from there they can interact and call events/functions in each other while still being decoupled.
-Object pool,because of time allocated to struggling with command pattern no implementation was given(again inside gdw game which I could not use, lab content did not assist with blueprint implementation)
-Falling tetris blocks, no collision in ui only








 (Odd) Observer explanation

Pseudocode diagram for implementing observer pattern in unreal engine using blueprints

-Create actor
-Open blueprint
-Search for which event you want to subscribe to
-Override this event/function (Anydamage for example)
-Add a bind event to (name of function) at the beginning of beginplay or a different time (should only be binded once)
-Drag out the event binding and create a custom event, this will create an event bound to your specified function/event
-Add game logic after the new event execution
-(optional) Add an unbind event node, preferably with a custom event called “unbind” that should only be executed once per bind.
