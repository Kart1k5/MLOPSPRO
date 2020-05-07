# MLOPSPRO
# JENKINS TASK

It is assumed that git ,docker(HTTPD) and jenkins arealready installed in your system 

step1 )create a item 1(PRODUCTION) that will keep eye on master branch any thing updated in master branch will automatically deployed on production system 

step2)create an item 1.1 which is depended on item 1 which launchs production docker if it is not launched .which is our production system .client can conect to it 

step 3)step1 )create a item 2(TESTING) that will keep eye on developer branch any thing updated in developer branch will automatically deployed on testing system

step 4)create an item 2.1 which is depended on item 2 which launchs test docker if it is not launched .which is our testing system .only my  quality testing team   can conect to it.

setp 5) create an item 3 which will merge master and developer branch . when QTT will test the testing system .if he/she find everything correct then he/she will build this item 3 . by using remote login access (like http://192.162.43.203:8080/job/token=redhat ) which is provided by jenkins . 

