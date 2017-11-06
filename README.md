# Performance profiling 

With performance, each website has its own issues.  So we cannot simply assume that a given piece of code is causing a problem and "fix" it.  We should see the problem for ourselves.  In addition, because improving performance can reduce code readability, there can be cost to over-optimizing for performance.

To protect against this, we employ performance profiling before making any changes.

### Performance Testing

One way in which we can keep a watchful eye on performance is to write tests.  

Use the `rails-perftest` gem to write performance tests.  There is a generator that allows you to get set up.  You may also need to install the `ruby-prof` gem and the `test:unit` gem.  To run the performance test, you can run `test:benchmark`.  

* [Benchmarking Rails](https://www.youtube.com/watch?v=eojUBB_8V_4&feature=youtu.be)

Watch the above video to learn more about using the `rails-perftest` gem.  How does the author of the video, Ryan Bates, determine which methods are causing the bottlenecks in the code, and then how does he go about making these changes?

### Performance Profiling

Another tool with an easy-to-use interface is called New Relic.  New Relic does require a signup on its webpage, however many of the features are free.  

Similar to in our performance tests, New Relic allows us to drill down to find bottlenecks in performance.  To see how to use and install New Relic, you can take a look at the following resources: 

* [New Relic Railscast](http://railscasts.com/episodes/161-three-profiling-tools)
* [New Relic TutsPlus](https://try.newrelic.com/rs/newrelic/images/Tuts%2B_Tutorials_GettingStarted30Minutes.pdf)

Finally, take a look at Skylight.  It is free, until your app exceeds 100,000 requests per month.  At that point, it costs $20 per month.

* [Skylight](https://www.skylight.io)

### The Terminal

We can see the performance directly in our applications.

<p class='util--hide'>View <a href='https://learn.co/lessons/performance-profiling'>Performance Profiling</a> on Learn.co and start learning to code for free.</p>
