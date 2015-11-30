Overview
========

In this project you will choose three things from a list of improvements for your web site.
Chose from the following list of topics:

1. Hosting on DigitalOcean
    
      Email me for an invite if you haven't already received one.
    
2. Caching with Memcached
    
      Install the Python memcached client https://pypi.python.org/pypi/python-memcached with pip and
      start a memcached docker image such as https://hub.docker.com/_/memcached/ .
      
      Use Django's caching interfaces to configure whole page caching for your app. Think about how and when
      to invalidate the cache'd content (after a certain amount of time? when the DB changes? something else?).
    
3. Unit tests
    
      Write unit tests for your models or experience services.Django has extensive support for writing unit tests
      including running tests against a new 'test' database so that your main database isn't changed
      by the test runs. You can load initial data into your test database using Django's 'fixtures'.
    
4. Integration tests
    
      Write integration tests using Selenium http://www.seleniumhq.org to test your web front end.
    
5. Performance testing
    
      Measure how fast your app will scale. This is a good project to do in combination with #1 above
      to measure how fast it runs on your laptop vs a DigitalOcean VM (it may not be as much different
      as you expect!). I recommend using JMeter http://jmeter.apache.org which is also available via
      a Docker image at https://hub.docker.com/r/hauptmedia/jmeter/ .
    
6. Load balancing
    
      Run multiple instances of your app tiers with a load balancer in front to distribute the load across
      all the instances. For example, if you have two copies of your web front end the load balance will
      sit in front of it, receive connections from browsers, and forward them on to one or the other
      of the web front end instances. 'pen' is a common and relatively simple one and is available 
      as a Docker image at https://hub.docker.com/r/galexrt/pen/ .
