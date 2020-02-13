
# command

gradle projects
gradle web:jettyRun
http://localhost:8081/todo

gradle build will launch the geb integration test.

Use this doc to configure gretty integration support:

https://akhikhl.github.io/gretty-doc/Integration-tests-support.html


selenium needs geckodriver to start firefox, download geckodriver here:

https://github.com/mozilla/geckodriver/releases

for this project, it uses v.26.0

I've added the gecko driver into the github.

After download, unzip the gekodriver into any directory, and set system property:

In GebConfig.groovy:

System.setProperty("webdriver.gecko.driver","/Users/shuaijie/Unix/commonLib/geckodriver");


this verison only works with gradle 5.1:


------------------------------------------------------------
Gradle 5.1
------------------------------------------------------------

Build time:   2019-01-02 18:57:47 UTC
Revision:     d09c2e354576ac41078c322815cc6db2b66d976e

Kotlin DSL:   1.1.0
Kotlin:       1.3.11
Groovy:       2.5.4
Ant:          Apache Ant(TM) version 1.9.13 compiled on July 10 2018
JVM:          1.8.0_231 (Oracle Corporation 25.231-b11)
OS:           Mac OS X 10.14.6 x86_64
