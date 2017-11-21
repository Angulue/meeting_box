# meeting_box
kind of skype in a phonebox , with blurred video of your interlocutor, old phone and a timer to mesure your conversation.

## Hardware
+ makey makey
+ a driing_sound.mp3
+ a Webcam with USB cable
+ a screen sand a server, or simply, a computer
+ 2 old phones, real or in cardboard

## Software
+ your computer prompt
+ any text editor, personnally I used sublimtext
+ download node.js
+ socket.io

## the experience ?
During Interaction 18, you could probably
bump into your future co-workers, your future boss,
or just some very interesting people.
In short, the event is a meeting time
and yet, it is not easy to engage a stranger
in a conversation.
The aim of the «meeting box experience»
is to prompt the discussion and encourage it.

## in 6 steps
1.Two connected «meeting box»
for two strangers in the crowd.

2.Go into the «meeting box». there,
you will see a phone, a screen,
and a camera. A timer is hidden in it.

3.You pick up the phone
in order to trigger a timer
and a blurred video appears.
you start to speak with somebody.

4.the conversation duration
directly influences the image blur.
It becomes clearer
and clearer as time goes by.

5.Now, you can see your
interlocutor on the screen.

6.Your curiosity is aroused
and your interlocutor’s one too.
you both decide to meet each other
for real.

## How to make the image blur become clearer and clearer as time goes by ?

1.You have to mesure time with your html thanks to the jquery function **setInterval()**.

The setInterval() method calls a function or evaluates an expression at specified intervals (in milliseconds).
The setInterval() method will continue calling the function until clearInterval() is called, or the window is closed.
The ID value returned by setInterval() is used as the parameter for the clearInterval() method.

```javascript
setInterval(function(){; }, 1000);

```
ok now you have to create a variable in order to say to your computer "every 100 milliseconds, the img become clearer of 0.15 px".

```
var interval;
   interval = setInterval(function(){ 
                blur -=0.15;
                }, 100)
```




