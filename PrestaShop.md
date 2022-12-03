**PrestaShop**


PrestaShop is an open-source eCommerce content management system that helps you easily create, manage, and design an online store for free. There are currently 300,000+ live websites using PrestaShop, making it the 6th most popular open-source platform.
The platform is known for its ease of use, making it suitable for business owners who want to make money online with minimum website development knowledge. 

**Install ability**:

To set up Presta shop on your local environment you must have to fulfill the following system requirements.

•	Registering a Domain Name

•	Finding a host

**Technical Requirements**

•	PHP 5.2 or Later

•	MYSQL 5.0 or Later 

•	UNIX/ Linux Hosting 

•	Apache Web Server 1.3 or later or nginx Web Server

•	Access codes to your FTP server, your MySQL database

•	Any modern Web browser (if using Internet Explorer: at least IE8)

•	At least 64 Mb of RAM on your Server

**Tools**

•	Any text editor

•	Any FTP client(File Transfer Protocol)


**Architecture:**

PrestaShop is based on three tier architecture.

• Object/data. Database access is controlled through files in the "classes" folder.

• Data control. User-provided content is controlled by files in the root folder.

• Design. All of the theme's files are in the "themes" folder.


**Requirements:**

1-	**Performance Efficiency**

It guarantees quicker development An firm may release the application to the market faster and programmers can utilise the most up-to-date and effective languages and tools for each tier because each tier can be created concurrently by various teams.
It ensures improved scalability. 

2-	**Reliability**

3-	**Security**

It fulfills the security attributes because the presentation tier and data tier can't communicate directly, a well-designed application tier can function as a sort of internal firewall, preventing SQL injections and other malicious exploits.

4-	**SOLID Principles**


**Clear and Modular Structure**

Prestashop has a clear and modular structure. A PrestaShop theme is a set of files which you can edit in order to change the look of your online shop. A classic theme is adopted.

**Security Attribute:**

You can integrate prestashop security suite with this open source platform to make it more secure. This module includes a firewall (WAF) to protect your site from XSS, SQL, HTML, and SHELL injection attacks. It implemets HTTP Security Headers, 2FA (Two-Factor Authentication). This extension helps you to protect your images and descriptions from being stolen by malicious people. Disable right-click, view page source, inspect element, and specific user key presses such as Ctrl+C, Ctrl+X, Ctrl+V, etc to prevent image/text theft.

**Modularity:**

More than 4,000 PrestaShop modules exist to help you to customize your online store, increase traffic, improve conversion rates and build customer loyalty. It consist of 88 built in modules. All these modules aim at providing basic optional features to help your store go to the next. These includes, payment, traffic management module, design and navigation, promotions and marketing etc.

**Maintainability:**

When writing open-source code, consistency is even more crucial because bug-fixing depends on the teeming millions of eyes on the code to actually find flaws and understand how to repair them. PrestaShop has provided details about its coding standard that must be followed for consistency. In short, having code consistency helps keeping the code readable and maintainable.

**Performance:** 

To optimize prestashop performance you need to

•	Choose the best web service hosting provider

•	Set up content delivery network(CDN)

•	Smarty Cache

•	Combine, Compress and Cache (The CCC section of the Performance section in your PrestaShop admin can be used to activate CSS, JS, and HTML compression, and caching, in addition to minifying HTML automatically)

•	Media Servers

•	Use latest PHP Version

•	Optimizing Images

**Stability**

Prestashop ensures stability as it is "well tested". In its latest version all three type of testing is done for automation i.e., **unit testing, integration testing, end to end testing,** .

Introducing Symfony in prestashop in its latest relaese allows us to get rid of the maintenance workload for a custom framework, which consumes a large amount of time that could be better spent working on what PrestaShop actually does best: managing a cart, handling orders, calculating prices and taxes, generating invoices, etc. Using a proven and popular open-source framework allows us to focus on our core business code with greater efficiency, while enjoying the stability of a globally recognized framework.


**Fault Tolerance**

A patch release is scheduled when a “trigger bug” is reported:

- A major bug in maintained branch
- A security issue in maintained branch
For example, let’s see 1.7.7.0 lifecycle:

Until PrestaShop 1.7.7.0 is released, the maintained branch remains 1.7.6.x.
This means that work on a new 1.7.6 release will start if a community contributor or the QA team reports a major regression in PrestaShop 1.7.6 or a security issue.
If minor or trivial regressions are reported for PrestaShop 1.7.6, they are scheduled to be fixed in **next minor version**. Minor or trivial bugs are considered not important enough to trigger a patch release process.

