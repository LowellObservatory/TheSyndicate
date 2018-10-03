## Ideas for "starter project" for the Lowell Software Syndicate

1. I was talking with Georgi and Teznie this morning when the subject of the DOL (DCT Operations Log) came up.
This is a program, written in LabView, that runs at the DCT and is used by the Telescope Operators to keep track
of events of various kinds that occur during the night’s observing run.  From our conversation, it seems that this
program has some deficiencies and could use improvement.  This program sends the “DCT Science Report” to the
dctops mailing list every morning.

   Because updating this application would be difficult for most of us because it is written in LabView, I propose that
we use this application as a first small project to write in Python using GitHub for project management.  The program
has connections to quite a few parts of the DCT systems and software, talking to the Broker to get TCS and weather information,
a graphical interface to gather information from the TOs, some hooks into a database, a connection to an email
client, etc.  We can also address some of the deficiencies in the current DOL in the new application.  Perhaps the new program
could send the final report directly to the Confluence page where these reports are archived.

   I think this application can be broken up into a few separate pieces that can be worked on by separate people and
then merged back into a whole.  This will lend itself to learning the collaborative aspects of GitHub.

   Of course this is just one possible idea for a learning program, others may be suggested at our meeting next Friday.

   There are lots of things to think about for the DOL, for example, will the application have a GUI written in PyQt5 or perhaps it
would work as a web application?  Will the program send out email in the morning as the current one does or could the gathered
information be made immediately available on a web page as it is accumulated during the night?

   We will need to have a couple of "DOL meetings” which should include the TOs,  to discuss the requirements as we go along.

   The User Manual for the current DOL is on Confluence at the URL below:

   https://jumar.lowell.edu/confluence/display/DCTDOC/DCT+Operations+Log+%28DOL%29+User+Manual

   If anyone has comments, please send them to me and/or bring them to the meeting next Friday.


2. Another idea, from Ryan, is to make an "electronic log" for astronomers that would allow them to make notes
on images as they come in from the instruments.

   Sample images of the current version of the code as of 2018 10 04; basically the top half would be chopped off and it'd just be maybe a clock of current/UTC time and then the data tables and notes section below
   
   ![logo](https://github.com/LowellObservatory/TheSyndicate/blob/master/Images/Screen%20Shot%202016-02-19%20at%205.38.03%20PM.png "CruiseDirector Notes")
   
   ![logo](https://github.com/LowellObservatory/TheSyndicate/blob/master/Images/Screen%20Shot%202016-02-19%20at%205.38.55%20PM.png "CruiseDirector DataLog")
   
