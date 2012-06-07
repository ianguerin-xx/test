###Deckard + Backbone and RequireJS

Check out blog post on this [here](http://plumlabs.us:81/blogs/show/19 "http://plumlabs.us:81/blogs/show/19")

Now running on nodejs + express, powered by [Roy](https://github.com/Valassis-Digital-Media/Roy "https://github.com/Valassis-Digital-Media/Roy")!

####To get running:
1. Get latest on Deckard2, Kilgore, & Roy. Put all three in ~/code/. So ~/code/Deckard2, ~/code/Roy, etc..
2. Install dependencies for all three (cd ~/code/Deckard2/ && npm install -d, etc..)
3. Install redis (I found Home Brew to be helpful, Mac Ports not so much..). With brew: 'brew install redis'
4. Start redis (with launchpad or manually).
5. Run the shell script ~/code/Deckard2/sh/restart-local-deckard.sh).
6. Go to Roy (http://localhost:3002/) and add an instance (Config must be in format of what Deckard2 expects).
7. Click 'view' next to the instance you just added.

####To optimize (minify/uglify js):
1. Run the optimizer.sh script (~/code/Deckard2/sh/optimizer.sh). The optimizer requires the RequireJS package, which can be easily installed using NPM. Make sure the optimizer (r.js) is in your PATH.

To run BDD tests:  
[mildred-grid](http://localhost:3000/scripts/apps/mildred-grid/tests/specRunner.html "http://localhost:3000/scripts/apps/mildred-grid/tests/specRunner.html")  
[facebook](http://localhost:3000/scripts/apps/facebook/tests/specRunner.html "http://localhost:3000/scripts/apps/facebook/tests/specRunner.html")  
[mildred-single-column](http://localhost:3000/scripts/apps/mildred-single-column/tests/specRunner.html "http://localhost:3000/scripts/apps/mildred-single-column/tests/specRunner.html")  
[mildred-next](http://localhost:3000/scripts/apps/mildred-next/tests/specRunner.html "http://localhost:3000/scripts/apps/mildred-next/tests/specRunner.html")  
[mildred-classic](http://localhost:3000/scripts/apps/mildred-classic/tests/specRunner.html "http://localhost:3000/scripts/apps/mildred-classic/tests/specRunner.html")  
[mildred-circle](http://localhost:3000/scripts/apps/mildred-circle/tests/specRunner.html "http://localhost:3000/scripts/apps/mildred-circle/tests/specRunner.html")  
[mildred-mobile](http://localhost:3000/scripts/apps/mildred-mobile/tests/specRunner.html "http://localhost:3000/scripts/apps/mildred-mobile/tests/specRunner.html")  
[mildred-savedotcom](http://localhost:3000/scripts/apps/mildred-savedotcom/tests/specRunner.html "http://localhost:3000/scripts/apps/mildred-savedotcom/tests/specRunner.html")

for detailed reporting change line 6 of \Deckard2\public\scripts\core\tests\jasmmine.js from jasmine.HtmlReporter() to jasmine.TrivialReporter()

####Most Recent Build:

####Test Results Graph:
[1]: http://build.plumlabs.us:8080/jenkins/job/Deckard2%20-%20DEV%20-%20Continuous%20(Pipeline%20Start)/test/trend
<img src="http://build.plumlabs.us:8080/jenkins/job/Deckard2%20-%20DEV%20-%20Continuous%20(Pipeline%20Start)/test/trend" title="Deckard2 Test Results Graph">


![Deckard2 Test Results Graph]([1] "http://build.plumlabs.us:8080/jenkins/job/Deckard2%20-%20DEV%20-%20Continuous%20(Pipeline%20Start)/test/trend")





