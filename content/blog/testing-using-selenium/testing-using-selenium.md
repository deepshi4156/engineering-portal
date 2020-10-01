In simple terms, one can define testing as checking or measuring the quality, reliability, or performance of a product before making it available for normal use. For example, most of the products ranging from a small pin to spacecraft are tested before they are made available. 

Today, we are in the world of technology dominated by software powered machines and applications. We expect them to work as we want every time and everywhere. Are we sure will they work? The answer lies in Software Testing.

Software Testing can be defined as investigating or checking the quality of software applications before their release to the user. The same testing is applicable even for web applications as most of the businesses today are internet or web-based. So why should we do testing for web applications? 

Imagine a scenario where you place an order on online shopping, but you are not able to track the status of your order. This may be due to a bug or error in the web application’s backend code. So there is a need for testing the code to avoid such bugs or errors. Selenium tool offers such testing for web applications.

Types of Software Testing
- Manual Testing
- Automation Testing

1. Manual Testing

   Traditionally software testing is carried out by Quality Assurance (QA) personnel by writing specific lines of code usually called, test cases. These test cases must be executed manually for every transaction using different types of attributes and datasets. The result of the test cases, either success or failure must be recorded manually. The major drawback of manual testing is the high chance of human errors while the repetition of test case execution which results in low product quality. 

2. Automation Testing

   The drawback of manual testing resulted in automation testing where a tool is used to execute test cases avoiding manual interference for every transaction. Further, we can configure the test cases so that they can be tested irrespective of operating systems, platforms and web browsers. The result of a test case can also be automated by scheduling it to a particular time of the day.

Here is the end to basics of testing, types of testing and their differentiation.  Now, the main focus of this blog is to introduce you the basics of Selenium, its components, comparison of Selenium with other top testing tools and concluding why selenium is best among them.

What is Selenium?

As said at the beginning of this blog, Selenium is an automation testing tool for web applications. It is a free source automation testing tool that is used to automate the tests on web browsers.

You may be wondering why only web applications and why not mobile and desktop software applications. There are other tools like Rational Functional Tester (RFT), Unified Functional Testing (UFT) (former QTP), Watir, Tricentis and so on for testing mobile and desktop software applications.

The first Selenium testing tool was developed by Jason Huggins in the year 2004 who was an engineer that time at ThoughtWorks. As a part of his work on testing web applications, Jason has realized that manual testing has become more inefficient due to repetitions of same test cases. 

This led to the creation of a JavaScript program called “JavaScriptTestRunner” to control browser actions automatically. Observing the potential in his idea, Jason made this JavaScript program as open-source and renamed it as Selenium Core.

Why the name Selenium?
The name Selenium has been adapted from a funny mail sent by Jason to his team. During the development of Selenium, there was a popular testing tool by a company named Mercury Interactive (it was the same company who developed QTP and later it was sold to HP). Since Selenium cures Mercury poisoning, Jason has suggested the same name. The team has adopted it and it is how Selenium got its present name.


Selenium Suite- It is proper to call Selenium as Selenium Suite since it is a collection of four different tools or components namely.
- Selenium Integrated Development Environment (IDE)
- Selenium Remote Control (RC)
- Selenium WebDriver
- Selenium Grid

1. Selenium Integrated Development Environment (IDE) - Selenium Integrated Development Environment (IDE) is the only simplest and easy to learn component or tool in the Selenium automation testing suite. IDE is a Firefox plug-in which can be installed easily to record and execute frequent test cases quickly. The user interactions with the web browser are recorded and test cases are created based on these recordings. You can playback these test cases repeatedly. Though Selenium IDE is simple, it cannot be used as a prototype for writing advanced test cases. 

Selenium IDE was initially created by Shinya Kasatani of Japan as a Firefox plug-in that records and playbacks the user-browser interactions. So initially Selenium IDE was also known as Selenium Recorder.  The other idea behind the development of Selenium IDE was to speed up the creation of test cases. Later in 2006, he donated this Selenium IDE to the Selenium Project.

2. Selenium Remote Control (RC) - Selenium Remote Control has been developed to overcome the issue of Same Origin Policy (SOP). Under this policy, a JavaScript code cannot access the elements of other domain that are different from its parent domain. For example, if a JavaScript program uses a code written for our site www.mindmajix.com, then SOP allows it to access the pages site such as mindmajix.com/all-courses or mindmajix.com/blog, prohibiting the access to other domains like google.com.

Before Selenium RC came into existence, testers used to locally install the copies of Selenium Core and web server with web applications to be tested so that, they both would belong to the single domain.  Observing this, Paul Hammant, another engineer at ThoughtWorks, created Selenium RC which turned out to be the permanent solution for the problem of the SOP. 

How does Selenium RC solve the SOP issue?
Selenium RC tricked the browser to believe that both Selenium Core and web server with the web application to be tested belong to the same parent domain. This has been achieved by involving a proxy HTTP server making RC as a dual-component tool – Selenium RC Server and Selenium RC Client.

Selenium RC was the first flagship testing tool of Selenium project which allows user preferred languages to write the test cases. Selenium RC 2.25.0 supports the following list of languages – 

- C
- Java
- Perl
- PHP
- Python and 
- Ruby
So, it is also called as Selenium 1. But, the major drawback of RC is, it consumes more time for every server communication taking hours of time to complete even a single test. 

Unfortunately, due to the depreciation, Selenium RC has been renamed as Selenium HQ and shifted to a legacy package. It means, we can still work with Selenium RC, but no support can be availed for it. You may be wondering what would be the replacement for RC. 

3. Selenium WebDriver
Selenium WebDriver was created by Simon Stewart in 2006 as the replacement for Selenium RC. Unlike IDE and RC, Selenium WebDriver provides an interface for creating and executing test cases. These test cases are created in such a way that, web page elements can be easily identified and necessary actions are performed. 

In 2008, Selenium WebDriver has been merged with Selenium RC and evolved as a more potent tool called as Selenium 2, keeping WebDriver as the core. So, Selenium WebDriver can be called as an upgrade version to RC as it employs a contemporary and consistent browser automation approach. WebDriver is much faster than RC because it directly calls the browser whereas RC needs a server to interact with the browser and depends on JavaScript for automated web application testing. Each web browser has its own WebDriver such as,

- Chrome Driver
- Gecko Driver (Firefox)
- HTM Unit Driver
- IE Driver
- Opera Driver and 
- Safari Driver
Selenium WebDriver supports the languages similar to that of Selenium RC
- C#
- Java
- Perl
- PHP
- Python and 
- Ruby
4. Selenium Grid - Selenium Grid is one of the Selenium testing tools used in combination with Selenium RC to execute test cases remotely. It was created by Patrick Lightbody to deal with the minimization of execution times of test cases. Selenium Grid was initially named as Hosted QA and was a part of Selenium 1. 

Selenium Grid uses Hub-Node design to support parallel execution of multiple test cases on multiple machines which are remotely located. In Hub-Node design, one machine is treated as Hub which controls the test cases running on different browsers inside different operating systems. The other machines are treated as Nodes on which test cases can be written in user preferred programming languages.

Here comes the end of the basic introduction of Selenium QA tool and its components. Now you will be introduced to other testing tools apart from the Selenium tool and why Selenium is the best among them by comparing the top five testing tools.

Why Selenium is the best automation testing tool? Before getting the answer to this question, you must be introduced to the top ten automation testing tools. The following is the list of top testing tools apart from Selenium testing tool. It includes both commercial and free source automation testing tools.

- Katalon Studios
- Unified Functional Testing (UFT) (former QTP)
- Test Complete
- Rational Functional Tester
- Watir
- Test Plant 
- Tricentis
- Ranorex
- Robot Framework

The following list showcases the advantages of Selenium testing tool that makes it best among other automation testing tools.
1. Selenium is an open-source automation testing tool and it is free of cost to use.
2. Selenium provides high tester flexibility to write advanced and complex test cases.
3. Supports test scripts written in any user-preferred languages such as C#, Java, Perl, PHP, Python, and Ruby
4. Supports test case execution on multiple operating systems such as Windows, Linux, Android, Mac, and iOS.
5. Supports testing on different web browsers such as Chrome, Firefox, Internet Explorer (IE), Opera, and Safari.
5. Test cases can be executed while the browser window is minimized.
6. Selenium supports parallel test execution.
7. Selenium can be integrated with TestNG and JUnit to generate test reports and manage test cases.
8. Selenium can be integrated with Jenkins, Docker, and Maven to attain continuous testing. 

Apart from the above advantages, Selenium testing tool has some shortcomings such as : 
- Selenium can test only web applications. It cannot test software applications and other desktop applications. 
- Selenium cannot access the web elements outside the web applications that are under test.
- No guaranteed user support is available. We have to depend on customer communities.
- Selenium independently does not support image testing. It must be integrated with Sikuli for image testing.

Conclusion - Selenium testing tool has both advantages and shortcomings in comparison to other automation testing tools. But, Selenium overshadows other testing tools in areas of –

Cost – Selenium comes at free of cost as it is an open-source testing tool.

Parallel Testing – Tester can execute test scripts on multiple machines simultaneously.

Flexibility – Selenium supports test scripts in multiple languages, execution on multiple browsers and operating systems.

On the conclusion note, the above three major features of Selenium and its different components made Selenium as one of the best automation testing tool.
