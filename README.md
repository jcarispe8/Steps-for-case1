# Steps-for-case1
1) setup git and circleCI
2) fork the branch
3) connect circleCI and run test
4) check results
5) read circleCI manuals
6) check if circle.yml is case sensitive
7) Circle.yml is faulty. Project runs without it.
8) looks like user's test does not reproduce any artifacts
and 
test:
 post:
   - mkdir -p $CIRCLE_TEST_REPORTS/junit/
   - find . -type f -regex ".*/target/surefire-reports/.*xml" -exec cp {} $CIRCLE_TEST_REPORTS/junit/ \;

gives no result

9)during creation of a video I've mentioned that there is a link to maven plugin that generates artifacts

10)update  pom.xml
