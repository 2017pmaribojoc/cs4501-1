# cs4501 Fall 2015
Internet Scale Applications
===========================

This course will provide a survey of methods for building large-scale internet websites and mobile apps. The intent is to build upon prior classes by explaining how theory meets practice. Topics covered will include scaling, security, large team software engineering, etc. There will be a series of cumulative course projects resulting in students building a working marketplace website. Weekly readings from industry and academic sources will complement the weekly lecture. 

Prerequisites
--------------

CS3240 Advanced Software Development or equivalent experience building Python/Django web applications is required. Understanding issues around persistence, databases, concurrency, networking etc along with Linux experience will be helpful in this class, but is not required.

A course project will be developed using Python, Django, MySQL, and Docker containers. A basic familiarity with HTML and CSS is preferred but not strictly required.

Project Overview
-----------------

You will work in a team of three to four students to build a working marketplace website. Marketplaces such as Airbnb, Uber, DonorsChoose, eBay, Etsy and Watsi are both highly profitable when they succeed and technically challenging to build. It's up to you to decide what kind of marketplace your team will build. Specific instructions for each project will be posted and linked below thoughtout the semester.

Due dates are listed below for each part of the project. These may be revised as the term goes on based on how everyone is doing. You will be graded as a team (unless unusual conditions warrant giving different grades). Grades will be based on: completeness of solution, correctness of solution, and being on time completing each assignment.

Course materials
-----------------

Syllabus and project assignments will be here in GitHub. Feel free to fork and send PRs with corrections, additions or any other changes you think would help fellow/future students.

Lecture slides are in Google drive at https://drive.google.com/folderview?id=0BzWAJQVnIIRYfk9JUmwtbUVKS1pqb0k0Q2ZYU3pPZ3gxV2VnVDctVU51VjFYTTVaR25xR3c&usp=sharing

Readings are listed for each week and should be completed BEFORE the week they are assigned so that we can discuss in class.

Course Topics (subject to revision as course progresses)
---------------------------------------------------------

1. Anatomy of the modern internet, websites and mobile apps (Friday 8/28 and Monday 8/31)
  - Trace a web request from browser to server and back
  - Overview of three/four tier app architecture
  - Overview of data center architecture: load balancers, switches, storage, servers
  - Overview of Model View Controller (MVC) design pattern
  - Overview of Docker and course project
  - Project: set up Docker container with Hello World Python/Django web app. Due Friday 9/4.
  - Resources: Django Getting Started docs https://docs.djangoproject.com/en/1.8/intro/ and https://docs.docker.com as well as  https://www.udacity.com/course/web-development--cs253 or http://www.codecademy.com/en/tracks/web if needed for HTML and CSS intro
2. Requirements and documentation (Friday 9/4)
  - User stories
  - Product requirement documents
  - Design and architecture documents
  - Project: Write user-stories and other documentation for project. Due Friday 9/11.
3. Service based architecture, part I (Monday 9/7)
  - Loosely coupled systems cooperating via services
  - Errors in the real world: failing gracefully and constantly
  - REST and API design
  - Project: Sprint 1: Start building site: create data models and service layer of project. Due 9/18.
  - Reading: Service Oriented Architecture at Netflix http://techblog.netflix.com/2012/06/netflix-operations-part-i-going.html , https://www.nginx.com/blog/microservices-at-netflix-architectural-best-practices/ and http://martinfowler.com/microservices/ . Optional, for more in-depth reading check out http://shop.oreilly.com/product/0636920033158.do
4. Databases (Friday 9/11 and Monday 9/14)
  - CAP theorem / Strong vs eventual consistency / Availability vs consistency
  - Common database use cases -- transactional data, logging, caches, etc
  - Sharding and partitioning
  - Case study: Cassandra
  - Project: Finish sprint 1
  - Reading: CAP theorem http://www.infoq.com/articles/cap-twelve-years-later-how-the-rules-have-changed and Eventual Consistency http://www.allthingsdistributed.com/2008/12/eventually_consistent.html, a counter-argument http://labouseur.com/courses/db/Stonebraker-on-NoSQL-2011.pdf and consistent hashing for sharding http://pdos.csail.mit.edu/papers/chord:sigcomm01/chord_sigcomm.pdf . Optional, Google Spanner http://research.google.com/archive/spanner.html
5. Service based architecture, part II: Multi-screen development for mobile and desktop (Friday 9/18 and Monday 9/21)
  - Proliferation of channels for consuming apps
  - App and experience logic server side vs client side
  - Responsive web design vs building different apps for different devices
  - Consistent experiences on mobile native, mobile web, desktop web, tablet, email etc
  - Service composition
  - Project: Sprint 2: Build view layer. Due 10/2.
  - Resources: Bootstrap http://getbootstrap.com/getting-started/ and Django templates https://docs.djangoproject.com/en/1.8/topics/templates/
6. Security (Friday 9/25 and Monday 9/28)
  - SQL injection and XSS
  - Denial of Service
  - Untrusted content (eg image exploits in UGC)
  - Stack smashing
  - Phishing
  - Internal IT and employees as attack vector
  - Project: Finish Sprint 2
  - Resource: Django security features: https://docs.djangoproject.com/en/1.8/topics/security/
  - Quiz #1 on Monday 9/28
15. Messaging and queing (Friday 10/2 -- No class Monday 10/5)
  - Integrating online and offline processing / Sync vs async
  - Queueing systems
  - Reading: Kafka at LinkedIn https://engineering.linkedin.com/kafka/kafka-linkedin-current-and-future and 
10. Search, Browse and Discovery (Friday 10/9 and Monday 10/12)
  - Product design strategies for navigating lots of inventory
  - Basics of information retrieval and search engines
  - Case study: ElasticSearch for site search backend
  - Recommendations and browsing as alternatives to search
  - Reading: Incorporating behavioral data in search http://research.microsoft.com/en-us/um/people/sdumais/SIGIR2006-fp345-Ranking-agichtein.pdf 
 8. Users and reputation (Friday 10/16)
  - User generated content (UGC): reviews, wiki posts, comments
  - Graph methods for reputation
  - Spam filtering
  - Case study: Amazon reviews
  - Reading: Analysis of StackOverflow http://www.cs.cmu.edu/~ymovshov/Papers/asonam_2013.pdf
7. Speed (Monday 10/19 and Monday 10/26 - No class Friday 10/23)
  - Importance of speed for users
  - What determines page load speed
  - Service orchestration and asynchronous processing
  - Content delivery networks
  - Case study: memcached
  - Reading: http://radar.oreilly.com/2009/07/velocity-making-your-site-fast.html
  - Resources: Python futures https://docs.python.org/3.4/library/concurrent.futures.html and Django cache APIs https://docs.djangoproject.com/en/1.8/topics/cache/
8. Testing and DevOps (Friday 10/30 and Monday 11/2)
  - Automated testing for services, web pages and mobile apps
  - Continuous integration and deployment
  - Monitoring and alerting
  - Infrastructure as code
  - Reading: Testing lifecycle at LinkedIn https://engineering.linkedin.com/41/testing-lifecycle-linkedin, continuous delivery at Facebook http://www.infoq.com/presentations/Facebook-Release-Process and dated but useful Google talk http://googletesting.blogspot.com/2008/11/clean-code-talks-unit-testing.html
11. TBD (Friday 11/6 and Monday 11/9)
12. Advertising (Friday 11/13)
  - Map of advertising ecosystem
  - Display advertising: targeting, trafficking and optimization
  - Search advertising: advertising as machine learning problem
  - Project: Sprint 6: Add user log in, account sign up, sign in/out etc. Due 12/4.
  - Reading: Ad Auctions (sections I and II in particular) http://users.cms.caltech.edu/~adamw/courses/241/lectures/search2.pdf
13. AB-testing and Analytics (Monday 11/16 and Friday 11/20)
  - Understanding the effect of product changes
  - Implementing tracking
  - Conversion funnels
  - AB testing and statistically significant changes
  - Hadoop / Spark for data analysis
  - Reading: AB testing at Spotify http://www.slideshare.net/alisarrafi3/ab-testing-at-spotify?next_slideshow=1 and http://www.slideshare.net/dj4b1n/ab-testing-pitfalls-and-lessons-learned-at-spotify-31935130 . Spark http://www.cs.berkeley.edu/~matei/papers/2010/hotcloud_spark.pdf . Optionally, can read more at https://play.google.com/store/books/details?id=VfVvAAAAQBAJ&source=productsearch&utm_source=HA_Desktop_US&utm_medium=SEM&utm_campaign=PLA&pcampaignid=MKTAD0930BO1&gl=US&gclid=COGFp6bcwMcCFQikNwodIH0IbA&gclsrc=ds
14. Traffic -- SEO, SEM, Social, Paid Marketing, Email (Monday 11/23)
  - Survey of driving traffic to a site / paid vs organic
  - Overview of SEO
  - Quantitative marketing, attribution models, ROI calculations
  - Case study: BuzzFeed
  - Reading: https://hbr.org/2007/05/viral-marketing-for-the-real-world
15. TBD (Monday 11/30, Friday 12/4, and Monday 12/7 -- No class Friday 11/27)
  - Quiz #2 on Friday 12/4

Grading
-------

Grades will be computed approximately as follows:  
25% class participation  
25% two quizzes  
50% class project  

Office Hours
-------------

Mondays 1-2pm in Rice 514. Contact the instructor if you would like to arrange another time to talk. Remember, it's always better to ask questions, bring up problems etc sooner vs later.
