xkcd-almamater-central-server
===================

This is a small web application that acted as a central hub for machines generating hashes for XKCD's almamater competition.


The Competition
===============

Randall Munroe, author of XKCD, posted a Skein hash digest.  The challenge was to try to get as close as possible to matching the hash he posted.


Our Solution
============

We handed out client software for anyone to run on as many of their own machines as possible.  The client made a call to this webserver which handed out a "block" of work.  Each block of work was simply a starting string value to start at.  The client would then iterate through strings and hashed them with the Skein algorithm.  If the client came across a hash beneath a certain threshold, it would report it back to the server where it could be viewed for submission.



How We Did
==========

We ended up in 9th place out of 182 submitted .edu domains.  

Some of the teams we beat included Harvard, Yale, Duke, Wisconsin, Rutgers, UC Davis, Purdue, Iowa, and Ohio State (not this time, Aaron Craft).

Some of the teams we lost to included Carnegie Mellon, MIT, Columbia, Cal Poly, Berkeley, Stanford, and Oxford.
