HAG Proposal
Contents
Introduction	1
Decomposition of client requirements	2
Recommended solution and justification of how client needs will be met	3
Risk log	3
Regulatory guidelines and legal requirements	7
Functional requirements	8
Non-functional requirements	10
KPIs	12
User Acceptance Criteria	12
Summary	16
Appendix A - research	16


Introduction
HAG is the client that has contracted me to develop their solution. They are a charity group standing for “Health Advice Group” who offer information and support on environmental health issues. They advise on how to deal with extreme weather conditions and mention health conditions based on environments and seasonal allergies such as asthma or hay fever. They specialise in conducting research based on different environments and displaying this to their clients to provide insightful information on health risks and issues.

HAG have tasked me to create a digital solution for them to help display environmental risks based on the chosen area and forecast its air quality and weather live while also listing health advice based on it. They do not provide live information based on different locations currently and give a live forecast of the weather. They only have advice on different conditions and fevers. The solution needs to allow the user to access a dashboard to search any area that they need advice or to view the air quality of and then they will be provided with advice alongside live displays of the weather.
Decomposition of client requirements
One of the client requirements is to provide advice on how to deal with health matters affected by weather and environmental conditions for example hay fever, asthma, colds and flu. There are quite a few different conditions that can be impacted by the weather and the environment. I am to tackle this requirement by including several health conditions on the website which can be searched for by the user. Once they have searched for a health condition the website will display advice and guidance on to deal with this condition. They will also have the option to get further advice from trusted websites eg. NHS website.
Another client requirement is access to a dashboard to monitor air quality data. I will fulfil this requirement by including a live map that they can use a search bar to change the location of. For example, in AccuWeather they have this with live icons displaying the air quality. I can use an API / script for the map to display the air quality on a dashboard which will be a separate page linked on the navbar. The map will be able to be enlarged for an even clearer and more accessible view and can be minimised with an icon on the top corner.
Another client requirement is advice on how to deal with health matters affected by weather and environmental conditions. I would like to create a separate page accessible on the navbar regarding health advice. There will be a small section at the top giving general health advice based on different weather conditions giving the user all information they need to tackle different conditions like ice and pollen. Common allergies for pollen would be hay fever so this would be touched upon in the section using bold writing, different headings to emphasise what is talking about what and a clear background colour to comprehend the text making this readable to different users.
Personalised health advice based on location is another requirement listed. This will be in the same tab as the previous one but in a separate section containing a search bar. The user will be able to enter their desired location and will receive flexible health advice based on what they entered. This will make the solution flexible and personalised to the user which is what HAG will need for an improved experience. Once their location is picked e.g Norway they will be given advice on how the cold conditions may affect their health. This could include colds and how to avoid them. Accuweather has a similar scheme in where activities listed and how easy it is to do them are listed. But instead, I will list health advice and conditions. I can do this by using API’s or linking a database of metrics that will be displayed.
Personal health tracking is the final requirement I must fulfil. I will put this in a separate page link on the navbar as ‘tracker’. There will be a calendar for the user to input any notes on health additionally that they would want to put. They must also enter 


Recommended solution and justification of how client needs will be met
I recommend the best way to meet the client requirements is to create a web-based solution. 
The website will include a page with a dashboard for monitoring air quality information.
On this page, the user will be able to enter a postcode or town/city location. The site will then search for the air quality data based on this information and display the data on the webpage. This will ensure that the client requirement has been met.
their location so that on the calendar, weather icons will be displayed on different days along with a temperature number which can be customised from C to F. The users must be signed in beforehand to access this though as it is personal to them and must be kept secure.
I have included a login and registration so that users can make a personal account. This is so that they may be able to access personal health advice tailored to them based on their location. This will also allow them to have a personal health tracker so having their own account that can only be securely accessed by them via email verification is a must.
The website will also include a dashboard page for weather forecasting to enter their own postcode or location. This will also list advice on how to deal with extreme weather based on their location and how they should manage their health. There will also be advice in general on health conditions and allergies caused by the current weather.
A website was chosen as this can be accessed on multiple devices making it accessible to multiple users. Websites can be made dynamically responsive for mobile, tablet and laptops. Accessibility features can also be included such as a dark mode toggle and language selector to be useful to those with visual impairments and those who speak different languages.

Risk log

Risk	Impact	Mitigation	New Impact	Other
Malicious/inappropriate use of the website by hacker -  we could have a hacker posing as a user to register and login to the website or create lots of fake accounts to access the website and gain unauthorised access	HIGH	To reduce the impact of this risk we ensure that all input to the website is validated. The registration page and login page will have validation features such as presence checks and format checks to ensure that data is valid and formatted correctly for the website. User accounts will be checked by authenticating them and verifying them with a valid email address.	MEDIUM	Project Manager
Intercepting data / man in the middle attacks – Hackers could intercept the firewall and sabotage data inputs between the user and the website for example their sensitive data like location or health conditions and account details.	HIGH	To reduce the likelihood of this, the database itself containing the user’s details must be secure and not be able to be accessed easily by third parties. We can use XAMPP and host it on a server only we have access to the data on it to be secured. All data transfers between users and the website must be encrypted to ensure any third parties cannot access the contents of it. We can use encryption keys that can only be decrypted by those who have access to the database.	MEDIUM	Project Manager
SQL injection – User data in our database is at risk from SQL query manipulations to inject malicious code. Entries in our database can be modified and authentication can also be bypassed due to user credentials being stored here.	HIGH	To mitigate this risk, we can keep the frameworks and libraries up to date so older versions cannot be exploited. Making sure error messages are not too detailed which can reveal structure in the database are not used and more simple errors are used instead such as ‘Access denied’.	MEDIUM	Project Manager
Anonymising data – Data could be modified such as sensitive data like health issues or user credentials losing a user’s identification such as their phone number or email.	HIGH	Encryption of data in the database with encryption keys only with those authorised will ensure that hackers cannot access the continents of data and manipulate them. 	MEDIUM	Project Manager
Inaccurate/unreliable weather data – Data could be inaccurate regarding weather. This can lose user trust or endanger lives if they blindly trust an inaccurate chart of data.	MEDIUM	Using multiple sources of data can help get a reliable statistic display such as satellite metrics, API weather services etc. Data models must also be up to date and reliable in today’s current standards to ensure that there is no incorrect statistics.	LOW	Project Manager
Incorrect Health Advice – This can endanger lives if they act on the wrong health advice. This could prove to be a huge loss if not mitigated professionally.	HIGH	Take extra care to ensure data displayed is reliable and up to date. Like the previous risk, multiple metrics will be used to gather conclusions.	MEDIUM	Project Manager
Localisation of data – If area entered is not specific, the data could be wrong or inaccurate due to different areas in a town	HIGH	Allow users to search area via postcode in their chosen reason to ensure data accuracy. Make sure data API’s and metrics used can allow this and have specific information on weather patterns and not general area wide. Disclaimers on data accuracy will also be added.	MEDIUM	Project Manager

Regulatory guidelines and legal requirements
GDPR – GDPR (General Data Protection Regulation) is a regulation that has been put in place for the entirety of the EU that lists out rules to follow on how organisations may collect, store and use the personal data of any clients they have. It aims to protect privacy and give users control of how their data Is used. Its principles consist of lawfulness and transparency, Purpose limitation, data minimisation, data accuracy, storage limitation and integrity and confidentiality. HAG will need to adhere to the principles of GDPR by ensuring that any personal data used is transparent meaning explicitly notified to the users in a privacy policy. Data must also only be used for a specified purpose by HAG, so to only be used to offer personal health advice to users. This can also be specified in the privacy policy. Data minimisation limiting data to only the purpose required so HAG will not collect more than needed. Data used must be up to date and accurate so user details must not be changed and kept up to date in the system. The data must be kept integral so not changed and confidential so that no one else can access it.
Health and social care Act 2012 – A legislation featured in the UK to shift decision making from the government itself to local organisations of healthcare. In general, it makes organisations must aim to provide high quality care and information to people. HAG will need to provide reliable weather data that is up to date and precise based on location. HAG must also provide links to other websites to further provide information to users and provide information based on user’s specific health conditions. If they require medicine information, HAG should link them to a more professional area where they may be able to get a prescription such as local clinics in the area.
Copyright and patents act: This act gives artists and online creators the right to own their own content to make sure it isn’t copied or used by anybody. It aims to give full control to those who copyright something. HAG will need to adhere to this law and must use images that are not copyrighted for example. Clips if used should also be checked for copyright and if HAG does wish to use something, they get permission and link the user such as in linked websites and articles for information. If permission is gained, they must be referenced.
W3C: an international organisation that develops open standards for web content. Its main purpose is to make sure all web content online is accessible, interoperable, secure and private and evolving. HAG will need to make sure that web content is accessible to everybody. This can be done by making sure I include dark mode toggles and multiple language toggles to make sure multiple users can access it. Interoperable. I will ensure the solution can be responsive and work the same on multiple devices like phones and tablets. I can use media queries for this.

Functional requirements
Requirement	Priority	Justification
The system will allow the user to register a new account	HIGH	The system must allow the user to register a new account so they can login to the system and access personalised health advice and dashboard to monitor their area’s weather / air quality
Weather forecast integration	HIGH	Accurate and accessible weather forecast information is part of the system’s purpose to provide insights and information regarding the weather in different areas making it flexible to the user.
Air Quality Dashboard	HIGH	Another system necessity to display different areas of the user’s choice and their air quality with live information
The system will allow the user to login to their account	HIGH	The system will allow the user to login to the system and allow them to view personalised information and dashboard
The system will allow users to access a page with FAQs	MEDIUM	This will not be a major priority as this will just allow the user to access a page on the website with frequently asked questions if they have any queries or difficulties with navigating the system
Personal health advice	HIGH	The system must be able to provide personal advice to user’s depending on their health conditions such as hay fever. They will be advised on what to do when pollen season is high or redirected to other web pages with more medical information.
Offline features	LOW	Not a necessity but can be good for users in desperate need to know or use the system. They won’t have live information but could have older or still be able to access health advice
Feedback	Low	Giving users the option to provide feedback can help build trust and improve the system in the future. Not a required element though.
Health tracker	Medium	Tracking for health isn’t a top necessity but would be useful for users who would like to track their health over time
Push Notifications	High	Notifications from the app will help notify the user of any emergency changes.
Emergency Alerts	High	Emergency alerts in real time of severe weather conditions will raise awareness and keep users safer. Information must be reliable
Encryption of user data	High	To comply with data protection laws the system must handle user data securely. To prevent interception, data in requests made will be encrypted.
Dashboard personalisation	Low	Allow the user to customise the layout of their dashboard to improve user engagement and satisfaction
Local area integration	High	Automatic location detection from
Date tracking	High	Allow users to see a calendar of dates and their weather or make any further warnings.
Educational tutorials	Medium	Integrating educational video links or article links regarding health advice can further be of use to users
Searched location history	High	This will save convenience if users are able to view their prior saved locations.
Local service integration	Low	Linking users to other services local to the area like a clinic or a hospital can give added intractability but is not essential.
Health recommendations 	High	Giving recommended advice is a must.

Non-functional requirements
Requirement	Priority	Justification
Green primary colour 	Medium	Reflects environment and sustainability which is HAG’s goal
Dark mode toggle	High	Dark mode toggle as an accessibility feature to those with visual impairments to comply with WCAG to ensure usability
Multi language selection	High	Complies with WCAG to ensure usability to all users.
The system must load in under 2.5 seconds	High	A fast load time will enhance the user experience and make it reliable.
Mobile responsiveness in under 760 px	High	Must be responsive to multiple devices to ensure anybody can access the system regardless of their device
System will be available and up 99% of the time ever year	High	Must be available at most times to ensure site reliability to users who want to access HAG services
The system must be scalable and handle up to 100000 users online at the same time initially but will be scalable to increase quickly in the future	High	Ensuring increased user count can be supported will help with the system’s growth.
The system must be compatible with multiple browsers e.g. safari and chrome	High	The system must be usable to all users no matter their preferred browser.
The system will optimise energy consumption for hosting servers to maintain sustainability goals of the environment.	Medium	Not a focus for the system itself but would align with HAG’s goals.
The system must have a response time of under 300 ms	High	Low response time will enhance system performance
User Privacy	High	GDPR will be complied with to ensure user private details are kept secure
The system will maintain good version control for new features	Medium	Not a focus but useful for the future of the website
Email support will be available 24 hours a day on the site’s launch	High	This will help maintain trust with users and ensure that the system is up to user standards
The system will resize text and allow user zooming	High	This will increase accessibility to users who may need more clarity.

KPIs
The website must have API weather display available 24 hours a day 7 days a week.
The website will load in a minimum of 5 seconds.
There will be a minimum of 5000 users in the first month of the website’s launch.
The website will retain at least 70% of users after the first month of the website’s launch.
The website will have an average user session duration of 10 minutes within the first month.
The website will have a minimum of 1500 interaction with the air quality dashboard.
The website will have 60% of users access the site with mobile devices after the 2nd month.
The website will track 1000 users’ health conditions within the first 2 months.
The website will resolve 90% of user complaints within the first month.
The website will have scheduled downtime no longer than once a month in which users will be notified in advance.

User Acceptance Criteria
User stories:
User	Action	Goal	User Acceptance Criteria
Customer	I would like to have a dark mode toggle on the website	This will aid my sight as my doctor has prescribed me to use darker / less blue light options on my devices	A dark mode switch must be visible on every page of the website in a suitable and easy manner. Switching between both modes will be fast and efficient
Customer	I would like to be able to access a map to monitor my air quality	This will help me understand better what parts of my country have better or worse air quality	The map will display air quality data by region and will allow users to search for specific locations on the map in real time.
Customer	I would like to able to track my health conditions based on my location and get personalised advice on this.	This will help me understand better what days my condition will be most vulnerable and what days I would be fine.	Users will be able to track symptoms over any basis of time and the system will give personally tailored advice based on their condition.
Customer	I would like to be able to access a weather forecast that will tell me about the weather based on my location.	This will help me understand what is going on with the weather for the next upcoming days better.	Weather forecast data will be shown based on the user’s location. Forecasts will be shown for up to 1 week ahead.
Customer	I would like a language selection on the website.	This will help me understand the site better as my native language is not English.	Language toggle will be shown on every single page of the website, and it will clearly be displayed.
Customer	I would like to receive daily notifications on the air quality.	This will help me prepare for the day by knowing if I need to take precautions.	Notifications can be toggled on and off and will be accurate based on that moment at a time specified by the user.
Customer	I would like the website to suggest activities for me to do based on the current weather and give me lifestyle advice.	This will help me improve my life as I will know what I will be able to do.	Activity suggestions will be shown and health advice on those activities will be shown
Customer	I would like a part of the website to explain how the air quality metrics function.	This will help me understand better the metrics that I am being shown on the website. 	An entire section on the air quality page will be clear and descriptive on what the air quality metrics are for.
Customer	I would like the website to link exterior medical help sites and clinics.	This will help me with treatments and medicine.	Exterior resource pages will be linked in the personal health advice page with local clinics also displayed. The links will be verified.
Customer	I would like the website to allow me to set health related tasks like medication or wearing a mask.	This will help me stay organised and keep on top of my health.	Users will be able to manage personal health related tasks with notifications also specified by the user.
Admin	I would like to be able to update general health advice based on weather when any changes arise.	This will allow the website to stay up to date.	Health advice will directly be editable on the dashboard. Changes will be live within 15 minutes.
Admin	I would like to update supported languages list.	This is so HAG can evermore appeal to more and more users.	Admins will be able to add new languages on the toggle via an admin drop down panel. Language files must be tested before use
Admin	I would like to be notified of any changes in air quality or weather that needs page updates.	This will also allow HAG to be up to date	Notifications will be clear and precise and will be sent via email.
Admin	I would like to be able to update and monitor the database.	This is so any changes or incorrect details can be corrected.	Admins can access security tools to change the database. Changes will automatically be audited.
Admin	I would like to manage user accounts and what they can access.	This can ensure efficient administration and data protection	Admins can manage user accounts and changes will take into effect immediately.
Admin	I would like to be able to update the privacy policy.	This will allow users to know that how their data is used.	Privacy policy updates will be live immediately and will notify users on any changes. Users will be allowed to access a FAQ about changes.
Admin	I would like to be able to change the website’s theme.	This can increase engagement with the site as it could be changed seasonally.	Admins can toggle between themes in the admin panel but can also create new ones. If liked, they will be available to use.
Admin	I would like to be able to backup and restore the website’s data 	This will allow data to be secure and ensure its availability and integrity.	Backups will be securely undergone to include all data.
Admin	I would like to create automatic backup schedules.	This will help the employees and admins know when backups will take place.	Admins can set up to monthly backup schedules and notifications will be sent a week prior.
Admin	I would like to test new features in an experimental environment.	This will make sure the solution is not disturbed, and users will not be disrupted	A simulated environment similar to the solution will be used to test new features and approve new changes to the solution itself.


Summary
This proposal gives a rough summary of what will be considered during development of the solution. User requirements are a focus and will be one of the first to be considered during development. I will try my best to meet all the requirements listed for HAG’s solution. Risks will also be touched upon to ensure that the solution is both secure and robust and thorough testing will also take place to ensure no errors are met before the solution is live. I will base this off of my test strategy. Thank you for reading my proposal, I will propose a solution that will meet all requirements. I have given my justifications for why I think a website solution is the most suitable proposition for HAG.
Appendix A – research

AccuWeather: 
AccuWeather is an example of how digital solutions can address the health sector’s needs, providing users with vital weather information to make informed health decisions.

 The website uses both hardware and software seamlessly, offering real-time forecasts, interactive weather maps, and alerts that can be customized based on location. This helps users stay ahead of extreme weather conditions and manage risks like heatwaves or cold snaps, which can impact conditions such as asthma or allergies. AccuWeather’s use of cloud-based technology ensures fast data processing and delivery, enhancing user experience. The site’s layout is designed for accessibility, with intuitive navigation, clear visuals, and easily readable text. It’s structured so that users can find necessary data quickly, regardless of their tech proficiency.
 
Radar API software
 
 The platform also integrates features that could inspire the development of similar tools, like personal health tracking that can be adapted for environmental health monitoring. Compliance with regulations such as data privacy and accessibility standards would be key when creating a solution like this. AccuWeather demonstrates how a user-centric, responsive platform can meet health sector needs, offering practical insights into applying technology for public health benefits. The Website itself does appeal less Nice due to its monotone colour scheme. It also does show health advice and what can be done by area.
 
Health tracking and advice based on different locations.

Plume Labs:

Plume Labs' digital solutions, like their *Air Report* app, show how technology can be applied to meet health needs by delivering real-time air quality information. The app helps users track pollution levels in their area and offers specific advice for protecting health, especially for those with respiratory issues. This is made possible by the integration of advanced sensors and cloud-based software, which provide reliable and timely updates. The app’s design is user-friendly and simple to navigate, making it accessible for users of all tech backgrounds. It includes key features such as air quality forecasts, pollution alerts, and health advice tailored to individual needs. This type of accessibility supports users with disabilities, promoting inclusive health tech.
 
Live world map

 Plume Labs’ model demonstrates how digital solutions, coupled with hardware tools, can be used to help people make informed decisions to avoid health risks linked to pollution. Any solution inspired by Plume Labs would need to follow strict data security and environmental health regulations. Their approach to blending digital tools with sensor technology provides valuable insight into creating effective health solutions. It has a universal page navbar that makes navigation easier aswell.


IQAir: 

IQAir is a platform focused on air quality monitoring, offering real-time data and personalized health advice based on location. The website’s interactive maps allow users to quickly check pollution levels, and its simple layout makes navigation straightforward. Clear sections, an effective search bar, and intuitive tools ensure that users can easily find relevant information. The site’s design emphasizes accessibility, with features that support diverse needs and ensure usability across various devices, including mobile phones. Navigation is smooth, and information is presented in an easy-to-digest format. While its reliance on real-time data requires accurate sources, it consistently delivers reliable insights. IQAir is a strong example of a user-friendly, digital health tool that effectively meets the needs of those managing environmental risks.

 
Animated map showing the flow of air and ratings by selected area.

 

Clean Nav design and logo making it clear.
 

The site does not include health advice by area though making it not meet one of the requirements of the project





 














	














