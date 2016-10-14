# SystemDesign

Stage 1: Basic CS Background
Good background knowledge on these topics helps
Operating systems
File system
virtual memory
paging
threads vs processes
concurrency 
Networking
TCP/IP stack
https
web services - REST, SOAP	
Database System
SQL vs NoSQL
hashing
indexing
master slave db
caching
Sharding
EAV based DBs
Web Architecture
distributed computing
cloud computing
load balancers
caching
proxy
Browsers

http://www.quora.com/What-is-the-difference-between-a-process-and-a-thread

Information on designing scalable apps:

david malans cs75 scalability talk Feel free to go through other lectures if needed.
https://www.youtube.com/watch?v=-W9F__D3oY4&list=PLmhRNZyYVpDmLpaVQm3mK5PY5KB_4hLjE&index=10
david huffman's talk , scaling up talk (Youtube link
https://www.youtube.com/watch?v=pjNTgULVVf4&list=PLVi1LmRuKQ0NINQfjKLVen7J2lZFL35wP&index=1
scalability for dummies

Stage 2: Intermediate Know about popular architecture

google
	search
	file system
	youtube
fb:
	graph search
	memcache
	instagram
	whatsapp
	
messaging frameworks
db
search, cache, video, cdn, image, website, 

Take notes.
See this talk: http://www.hiredintech.com/system-design/the-system-design-process/ and develop a process for how to answer such questions .

Stage 3: Have a general template:
These are the steps I go through mentally in the interviews, followed by actual interview experiences:

    a) Be absolutely sure you understand the problem being asked, clarify on the onset rather than assuming anything
    b) Use-cases. This is critical, you MUST know what is the system going to be used for, what is the scale it is going to be used for. Also constraints like requests per second, requests types, data written per second, data read per second.
    c) Solve the problem for a very small set, say 100 users. This will broadly help you figure out the data structures, components, abstract design of the overall model.
    d) Write down the various components figured out so far and how will they interact with each other.
    e) As a rule of thumb remember atleast these :
        1.processing and servers
        2.storage
        3.caching
        4.concurrency and communication
        5.security
        6.load balancing and proxy
        7.CDN
        8. Monetization: if relevant, how will you monetize? eg . What kind of DB (will mysql do ? or nosql fits btr? ), do you need caching (almost always !) and how much, is security a prime concern?
    f) Special cases for the question asked. Eg say designing a system for storing thumbnails, will a file system suffice? What if you have to scale for facebook or google? Will a nosql based db work?
    g) After I have my components in place, what I generally try to do is look for minor optimization in various places according to the usecases, various tradeoffs that will help in better scaling in 99% cases.
    h) Scaling out or up
    i) Check with the interviewer is there any other special case he is looking to solve? Also it really helps if you know about the company you are interviewing with, what its architecture is, what will the interviewer have more interest in based on the company and what he works on?

know about the companies work:
Go through the engineering blog of the company you are interviewing in (or if its a startup go through the link of the company closest to yours)


Stage 4: common designs questions
Try attempting the FAQs on design using the template.
"Practice, whiteboard, mocks, revice"

Design Twitter:
http://blog.gainlo.co/index.php/2016/02/17/system-design-interview-question-how-to-design-twitter-part-1/




































References:

https://github.com/checkcheckzz/system-design-interview/blob/master/README.md
https://github.com/shashank88/system_design
https://github.com/filipegoncalves/interview-questions/tree/master/systems_design
https://github.com/andreis/interview
http://blog.gainlo.co/index.php/2015/10/22/8-things-you-need-to-know-before-system-design-interviews/
http://superherojs.com/#browser