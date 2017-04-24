# DoclerTest
# Description 
These automated testcases were created in C# using Selenium, Specflow and NUnit3, in Visual Studio 2017 Community. 
Number of requirements: 12
Number of test cases: 7
Parallel execution is possible, however there are only 2 threads due to the number of testcases.


# Requirements 
- The latest Chrome browser (58)
- Visual studio 2017 Community
- Selenium (included in library)
- The latest Chromedriver (included in library)

# How to use
1. In Visual Studio 2017 click on Open.
2. Then click on Open Solution.
3. Select Solution2 and click on open.
4. Once the Solution loaded, build it.
5. Run the tests.

# Troubleshooting
- Specflow is missing (http://toolsqa.com/specflow/set-up-specflow/)
- Selenium is missing (https://www.joecolantonio.com/2013/01/18/selenium-webdriver-using-chrome-webdriver-in-visual-studio-c/)
- Nunit is missing (https://marketplace.visualstudio.com/items?itemName=NUnitDevelopers.NUnit3TestAdapter)

# Known issues: 
chromedriver process won't stop after the testcase is finished.
I tried to kill the process, however that caused issues with the parallel execution.
Possible solution: keep track of the PIDs of the chromedrivers which the testcase starts and stop the chromedriver with the corresponding PID.
