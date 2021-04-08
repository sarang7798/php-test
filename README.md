#history for the run.
    1  launch.sh
    2  oc new-project pro1
    3  oc project
    4  oc new-app https://github.com/sarang7798/php-test.git
    5  oc get pods-w
    6  oc get pods -w
    7  oc get pods -o wide
    8  oc get svc
    9  curl 10.128.0.23
   10  curl 10.128.0.23:8080
   11  curl 172.30.223.27
   12  oc get svc
   13  oc get pods -o wide
   14  curl 10.128.0.25
   15  curl 10.128.0.25:8080
   16  oc get svc
   17  curl 172.30.223.27
   18  curl 172.30.223.27:8080
   19  git clone https://github.com/sarang7798/php-test.git
   20  ls
   21  cd php-test/
   22  ls
   23  vim index.php
   24  git add .
   25  git commit -m "this is coming from rhel"
   26  git push origin master
   27  oc get pods
   28  oc start-build php-test
   29  oc get pods
   30  oc get pods -o wide
   31  oc get pods -w
   32  oc get pods
   33  oc get pods -o wide
   34  curl 10.128.0.28:8080
   35  history


#history2 for the run.

#**We are pushing new code to git and then again getting the same code and deploying that one to create new pods for the same name.**

    1  launch.sh
    2  git clone https://github.com/sarang7798/php-test.git
    3  cd php-test/.git/
    4  ls
    5  cd ..
    6  ls
    7  cd ..
    8  rm -rvf php-test/
    9  ls
   10  oc new-app https://github.com/sarang7798/php-test.git
   11  oc get pods -w
   12  oc get pods
   13  oc get pods -o wide
   14  curl 10.128.0.25
   15  curl 10.128.0.25:8080
   16  git clone https://github.com/sarang7798/php-test.git
   17  cd php-test/
   18  ls
   19  vim index.php
   20  git add .
   21  git commit -m "3rd try"
   22  git push origin master
   23  oc start-build php-test
   24  oc get pods -w
   25  oc get pods
   26  oc get pods -o wide
   27  curl 10.128.0.28
   28  curl 10.128.0.28:8080
   29  history
