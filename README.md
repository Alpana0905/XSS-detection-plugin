**XSS ATTACK DETECTION EXTENSION**

GENERALIZED IDEA OF OUR PROJECT->
With the increased use of the internet, web applications and websites are becoming more and more common due to which cyber-attacks on web applications and websites are also increasing. 
Of all the different types of cyber-attacks on web applications and websites, XSS (Cross-Site Scripting) attacks are one of the most common forms of attack. 
*An attacker who exploits a cross-site scripting vulnerability is typically able to read any data that the user can access, capture the user's login credentials, impersonate or masquerade as the victim user. 
*XSS attacks enable attackers to inject client-side scripts into web pages viewed by other users. 
*The existing attack detection strategies have failed miserably in most of the situations. Moreover, users have also not taken much care of configuring their browsers securely, using available extensions and plugins. 
*The scripts are also executed automatically without the user’s permission unless he disables it. 
*The users therefore need to protect themselves from these vulnerabilities hence the detection of XSS attacks is very important.
*So, we decided to make a plugin which detects whether the site is XSS vulnerable or not in real time by penetrating inside the site’s code and inserting our JS code to check if it returns any information or not. 
*If we get any valuable information as a result of the code we inserted, then the site is XSS vulnerable otherwise it is not XSS vulnerable.

DETAILED PROCESS->
•	The user or victim will first log into his account.
•	The user must next download and install the XSS Extension on his or her web browser.
•	The user must open any webpage after installing the extension on their browser.
•	The URL of the currently open tab will be captured by the extension.
•	The extension sends it to our created backend.
•	It extracts the URL in the backend and passes it to the scanner python file.
•	The Beautiful Soup library in the python code detects the forms on the webpage.
•	A dummy JavaScript is created to inject into the webpage.
•	All the forms present on the webpage are traversed thoroughly.
•	The details of the forms like their action, method and inputs are extracted.
•	The form is then submitted using all the details we got and insert JavaScript in the text input field.
•	If the script gets inserted to the webpage, then, it is vulnerable, otherwise it is not vulnerable.

IMPLEMENTATION TECH STACK->
•	Python (Beautiful Soup)
•	Node JS (Express) 
•	HTML CSS

![flowchart](https://github.com/Alpana0905/XSS-detection-plugin/assets/78347586/11d62a8b-dd5a-4d40-9550-e971876ec28d)
