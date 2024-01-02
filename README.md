# AIdeas
<!-- This is the markdown template for the final project of the Building AI course, 
created by Reaktor Innovations and University of Helsinki. 
Copy the template, paste it to your GitHub README and edit! -->

# Project Title

“Your Musical Instrument Tutor”
Final project for the Building AI course

## Summary

“Your Musical Instrument Tutor” - checks how your musical instrument training is going, and gives you tips on how to proceed, based on your actual current level.

 “Your Musical Instrument Tutor” is a TinyML solution – to run on an embedded system, using a pre-trained AI, with no run-time connection to the world.

## Background

The problem that my idea will solve may be divided in two parts:

1)	When training to learn a musical instrument, you need feedback. You would often like a more frequent feedback than those once a week lessons with your teacher. Here is the always available teacher for you!
2)	Also: the tinyML part of the idea solves other problems: - You can use can use the solution in a cabin in the woods without mobile connection, or, in a sound-proofed thick-walled cellar or shed where your siblings cannot hear or disturb you.

The problem part 1) is common for anyone who is learning an instrument. Those are quite many – and they would be more, if more were given the chance. This idea does give more people more chances to learn a musical instrument, and learn it better, faster! - The problem part 2) is  also something that not all but indeed some musical instruments learners would benefit from. It may be for several reasons that you would benefit from being able to work without an Internet/mobile connection. Cost, battery saving, and of course to eliminate the need for a working mobile connection, mobile prescription, mobile per se, etc.

To get more people to exercise a musical instrument in a more rewarding way, would give them a chance to grow, to relax, to feel good. This in a next step may do something more: to contribute to our society’s wellbeing. 


## How is it used?

“Your Musical Instrument Tutor” may be used by anyone who wants more feedback on their musical instrument training, than they otherwise would have. Their today may include lack of resources of some type(s): available teacher time, available practice time when there is a suitable location, etc.

If the ML training data comes from an actual teacher, this affects teachers who can sell fewer lessons to some students. On the other hand, teachers can now reach other students than before. Also, the “good spiral” from contented students will make the market grow even more just because of this.


## Data sources and AI methods

Data for one implementation of this idea: - Your teacher records the music you are to train. (One can imagine more elaborate other implementations and related data sources. That would complicate this idea unnecessarily for a first version of the idea.)

AI and other techniques that may be helpful:
-	From the recorded audio, extract the features that are relevant to us. That would include tone frequency/-ies, tone length/-s, and step by step more as found useful. “Tone pictures” – not too big, but also not too small. 
-	Convert the features you have extracted, to spectrograms. (Frequency/time data.)
-	Then, feed the spectrograms to an ML framework, specific for an embedded system.
-	From this ML framework, you get a “command recognizer”.
-	And this in turn gives you a “command responder” which will handle your own recorded music training session, for this concerned tune.

TFLite for microcontrollers may be useful here. 
Some type of neural network may be used - like a transformer. But for the fun of it - what will happen if we test even simpler ways like logistic regression? 
  
The ML solution is not meant to be spread to other than the specific teacher/student pair. It is still “their lesson” with the same material as for an IRL lesson. That should help to avoid immaterial property rights problems which would otherwise occur.


## Challenges

To identify which features to extract, will be the first and big challenge. The way to do this would be to try, and try again. 

This project (in its first version, described above) is not altogether flexible. It requires planning: which tune do I need my teacher to record, before I practice with this solution? The student (and teacher) need be motivated enough to work past this obstacle. The solution need be user friendly enough to encourage them to do this.

This project also requires some handling by teacher/student, for to train the ML with a certain tune, when it is new to the system. Again, user-friendliness is essential here, for the project.

(A later version of the project may train on all sorts of recordings – but when it comes to intellectual property right etc, this gets far more complicated than the first solution involving just a teacher and a student.)

As this is not a safety or security focussing problem and solution, it is alright that there are some limitations to it. 
To use the solution, you do need some basic equipment which is still though fairly cheap per se. For example, you may use an Arduino with some simple power source, and a couple of reasonably simple microphones.


## What next?

This project could grow most easily and most natural if some bigger party in some concerned branch of business would be involved. Say, a manufacturer of instruments, or a music business company, or an academic institution. This way already existing parties with a lot of relevant knowledge, and other resources, could enhance the project. 

To make the project an open source project would also be one way to go. 


## Acknowledgments

- A very good source of inspiration is TinyML, and renowned schools and courses like https://pll.harvard.edu/course/fundamentals-tinyml.

- [TF Lite for microcontrollers](https://www.tensorflow.org/lite/microcontrollers)
