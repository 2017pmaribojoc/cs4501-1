# cs4501 Spring 2016
Internet Scale Applications
===========================

This course will provide a survey of methods for building large-scale internet websites and mobile apps. The intent is to build upon prior classes by explaining how theory meets practice. Topics covered will include scaling, security, large team software engineering, etc. There will be a series of cumulative course projects resulting in students building a working marketplace website. Weekly readings from industry and academic sources will complement the weekly lecture. 

Prerequisites
--------------

CS3240 Advanced Software Development or equivalent experience building non-trivial Python/Django web applications is required. Understanding issues around persistence, databases, concurrency, networking etc along with Linux experience will be extremely helpful in this class.

A course project will be developed using Python, Django, MySQL, and Docker containers. A basic familiarity with HTML and CSS is preferred but not strictly required.

Project Overview
-----------------

You will work in a team of three to four students to build a working marketplace website. Marketplaces such as Airbnb, Uber, DonorsChoose, eBay, Etsy and Watsi are both highly profitable when they succeed and technically challenging to build. It's up to you to decide what kind of marketplace your team will build. Specific instructions for each project will be posted and linked below thoughtout the semester.

Due dates are listed below for each part of the project. These may be revised as the term goes on based on how everyone is doing. You will be graded as a team (unless unusual conditions warrant giving different grades). Grades will be based on: completeness of solution, correctness of solution, and being on time completing each assignment.

Course materials
-----------------

Syllabus and project assignments will be here in GitHub. Feel free to fork and send PRs with corrections, additions or any other changes you think would help fellow/future students.

Lecture slides are in Google drive at https://drive.google.com/folderview?id=0BzWAJQVnIIRYfk9JUmwtbUVKS1pqb0k0Q2ZYU3pPZ3gxV2VnVDctVU51VjFYTTVaR25xR3c&usp=sharing Note that prior semester's slides can be found here for future lectures, but they may be out of date / subject to update this semester. Generally, the further out a lecture is the more likely that the slides have not been reworked for this semester.

Readings are listed for each week and should be completed BEFORE the week they are assigned so that we can discuss in class.

Course Topics (subject to revision as course progresses)
---------------------------------------------------------

1. Anatomy of the modern internet, websites and mobile apps (Weds 1/20 and Monday 1/25)
  - Trace a web request from browser to server and back
  - Overview of three/four tier app architecture
  - Overview of data center architecture: load balancers, switches, storage, servers
  - Overview of Model View Controller (MVC) design pattern
  - Overview of Docker and course project
  - Project: set up Docker container with Hello World Python/Django web app. Due Weds 1/27. https://github.com/thomaspinckney3/cs4501/blob/master/Project1.md
  - Resources: Django Getting Started docs https://docs.djangoproject.com/en/1.8/intro/ and https://docs.docker.com as well as  https://www.udacity.com/course/web-development--cs253 or http://www.codecademy.com/en/tracks/web if needed for HTML and CSS intro
2. Requirements and documentation (Weds 1/27)
  - User stories
  - Product requirement documents
  - Design and architecture documents
  - Project: Write user-stories and other documentation for project. Due Monday 2/1.
3. Service based architecture, part I (Monday 2/1)
  - Loosely coupled systems cooperating via services
  - Errors in the real world: failing gracefully and constantly
  - REST and API design
  - Reading: Service Oriented Architecture at Netflix http://techblog.netflix.com/2012/06/netflix-operations-part-i-going.html , https://www.nginx.com/blog/microservices-at-netflix-architectural-best-practices/ and http://martinfowler.com/microservices/ . Optional, for more in-depth reading check out http://shop.oreilly.com/product/0636920033158.do
  - Project: Start building site: create data models and service layer of project. Due Monday 2/15. https://github.com/thomaspinckney3/cs4501/blob/master/Project2.md
4. Databases (Monday 2/8 and Weds 2/10 - No class Weds 2/3)
  - CAP theorem / Strong vs eventual consistency / Availability vs consistency
  - Common database use cases -- transactional data, logging, caches, etc
  - Sharding and partitioning
  - Case study: Cassandra
  - Reading: CAP theorem http://www.infoq.com/articles/cap-twelve-years-later-how-the-rules-have-changed and Eventual Consistency http://www.allthingsdistributed.com/2008/12/eventually_consistent.html, a counter-argument http://labouseur.com/courses/db/Stonebraker-on-NoSQL-2011.pdf and consistent hashing for sharding http://pdos.csail.mit.edu/papers/chord:sigcomm01/chord_sigcomm.pdf . Optional, Google Spanner http://research.google.com/archive/spanner.html
5. Service based architecture, part II: Multi-screen development for mobile and desktop (Monday 2/15 and Weds 2/17)
  - Proliferation of channels for consuming apps
  - App and experience logic server side vs client side
  - Responsive web design vs building different apps for different devices
  - Consistent experiences on mobile native, mobile web, desktop web, tablet, email etc
  - Service composition
  - Project: Build view layer. Due Monday 2/29. https://github.com/thomaspinckney3/cs4501/blob/master/Project3.md
  - Resources: Bootstrap http://getbootstrap.com/getting-started/ and Django templates https://docs.djangoproject.com/en/1.8/topics/templates/
6. Security (Monday 2/22 and Weds 2/24)
  - SQL injection and XSS
  - Denial of Service
  - Untrusted content (eg image exploits in UGC)
  - Stack smashing
  - Phishing
  - Internal IT and employees as attack vector
  - Resource: Django security features: https://docs.djangoproject.com/en/1.8/topics/security/
15. Messaging and queing (Monday 2/29 and Weds 3/2)
  - Integrating online and offline processing / Sync vs async
  - Queueing systems
  - Reading: Kafka at LinkedIn https://engineering.linkedin.com/kafka/kafka-linkedin-current-and-future and 
  - Quiz #1 on Weds 3/2
  - Project: user accounts and user generated content. Due Monday 3/21. https://github.com/thomaspinckney3/cs4501/blob/master/Project4.md
10. Search, Browse and Discovery (Monday 3/14 and Weds 3/16 - No class Monday 3/7 or Weds 3/9)
  - Product design strategies for navigating lots of inventory
  - Basics of information retrieval and search engines
  - Case study: ElasticSearch for site search backend
  - Recommendations and browsing as alternatives to search
  - Reading: Incorporating behavioral data in search http://research.microsoft.com/en-us/um/people/sdumais/SIGIR2006-fp345-Ranking-agichtein.pdf 
8. Users and reputation (Monday 3/21)
  - User generated content (UGC): reviews, wiki posts, comments
  - Graph methods for reputation
  - Spam filtering
  - Case study: Amazon reviews
  - Reading: Analysis of StackOverflow http://www.cs.cmu.edu/~ymovshov/Papers/asonam_2013.pdf
  - Project: search. Due 4/4 https://github.com/thomaspinckney3/cs4501/blob/master/Project5.md
7. Speed (Weds 3/23 and Monday 3/28)
  - Importance of speed for users
  - What determines page load speed
  - Service orchestration and asynchronous processing
  - Content delivery networks
  - Case study: memcached
  - Reading: http://radar.oreilly.com/2009/07/velocity-making-your-site-fast.html
  - Resources: Python futures https://docs.python.org/3.4/library/concurrent.futures.html and Django cache APIs https://docs.djangoproject.com/en/1.8/topics/cache/
8. Testing and DevOps (Weds 3/30 and Monday 4/4)
  - Automated testing for services, web pages and mobile apps
  - Continuous integration and deployment
  - Monitoring and alerting
  - Infrastructure as code
  - Reading: Testing lifecycle at LinkedIn https://engineering.linkedin.com/41/testing-lifecycle-linkedin, continuous delivery at Facebook http://www.infoq.com/presentations/Facebook-Release-Process and dated but useful Google talk http://googletesting.blogspot.com/2008/11/clean-code-talks-unit-testing.html
  - Project: Enhancements. Due 4/18. https://github.com/thomaspinckney3/cs4501/blob/master/Project6.md
11. TBD (Weds 4/6 and Monday 4/11)
12. Advertising (Weds 4/13)
  - Map of advertising ecosystem
  - Display advertising: targeting, trafficking and optimization
  - Search advertising: advertising as machine learning problem
  - Project: Sprint 6: Add user log in, account sign up, sign in/out etc. Due 12/4.
  - Reading: Ad Auctions (sections I and II in particular) http://users.cms.caltech.edu/~adamw/courses/241/lectures/search2.pdf
13. AB-testing and Analytics (Monday 4/18 and Weds 4/20)
  - Understanding the effect of product changes
  - Implementing tracking
  - Conversion funnels
  - AB testing and statistically significant changes
  - Hadoop / Spark for data analysis
  - Reading: AB testing at Spotify http://www.slideshare.net/alisarrafi3/ab-testing-at-spotify?next_slideshow=1 and http://www.slideshare.net/dj4b1n/ab-testing-pitfalls-and-lessons-learned-at-spotify-31935130 . Spark http://www.cs.berkeley.edu/~matei/papers/2010/hotcloud_spark.pdf . Optionally, can read more at https://play.google.com/store/books/details?id=VfVvAAAAQBAJ&source=productsearch&utm_source=HA_Desktop_US&utm_medium=SEM&utm_campaign=PLA&pcampaignid=MKTAD0930BO1&gl=US&gclid=COGFp6bcwMcCFQikNwodIH0IbA&gclsrc=ds
  - Project: Hadoop. Due 5/2.
14. Traffic -- SEO, SEM, Social, Paid Marketing, Email (Monday 4/25)
  - Survey of driving traffic to a site / paid vs organic
  - Overview of SEO
  - Quantitative marketing, attribution models, ROI calculations
  - Case study: BuzzFeed
  - Reading: https://hbr.org/2007/05/viral-marketing-for-the-real-world
15. TBD (Weds 4/27, Monday 5/2)
  - Quiz #2 on Friday 4/27

Grading
-------

Grades will be computed approximately as follows:  
10% class participation  
30% two quizzes  
60% class project  

Office Hours
-------------

The teaching staff for this semester are:

  - Tom Pinckney (lecturer) tp3ks@virginia.edu
  - David Amin (TA) dma3fq@virginia.edu
  - Ian Zheng (TA) yz9fy@virginia.edu
  - Daniel Mace (TA) dfm4ff@virginia.edu

There will be one set of office hours for project questions and demos and another time for general class questions. Each project is two weeks. During the first week a project is assigned, the project review hours will be about how to do the project. During the second week that each project is assigned, the project hours will include mandatory demos of your team's progress. If you are unable to make the demo hours, please contact the teaching staff to arrange an alternative time.

   - Project review, help, and demo hours: Weds 1-2:30 and Sunday 3-4:30 (lead by TAs). Location TBD.
   - General Q&A Monday 2:30 - 3:30 (led by Tom). Location TBD.

There is also always help from the teaching staff and your fellow classmates through slack at https://cs4501-isa.slack.com

Remember, it's always better to ask questions, bring up problems etc sooner vs later.
