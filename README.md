# Playwright-Medibank
This repo contains Playwright with mocha-chai for UI test cases as per assessment questions

## Medibank Test Scenario

Task 1: Select a public website and write a couple of test scripts in &quot;Playwright&quot; Test automation tool
covering below framework principles
 Input Data reading from external file (your choice of file format)
 POM
 Reporting in html / CICD compatible report
 Execution command line options to run on variety of supported browsers
Tests can be small, navigating to a few pages. Interacting with elements on page, Login (if possible)
and validation. You can use language as JavaScript or Typescript to create scripts.

Answers:

1. Login data is read from testData.csv under data folder under test
2. POM has been craeted for login page and product list page
3. Report is being generated in html & json format -- mochawesome report. open the .html extension file under mochawesome-report through 
   file explorer / finder or directly in chrome using "file:/// <file path>"
4. Execution commands to run test on diferrent browser is as below:

## Execute Tests

Run below commands from CLI to run tests on different browsers

	"testChrome": "NODE_ENV=chrome npx mocha test/testChrome.js -- --browser chrome --reporter mochawesome",
    "testFirefox": "NODE_ENV=firefox npx mocha test/testChrome.js ----browser firefox --reporter mochawesome",
    "testSafari": "NODE_ENV=safari npx mocha test/testChrome.js -- --browser safari --reporter mochawesome",	

Note: The command can be configured to execute test from single command and set NODE_ENV from CLI directly

