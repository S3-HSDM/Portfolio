# Authentication

## What and Why
For my IP I created a Hearthstone Deck Maker. In this application is it possible for everyone to view all available cards and created decks, but the created decks should only be able to be edited by the user that created it. Also to keep the site up-to-date admins or moderators should be able to create, edit or delete Cards, which normal users should have no access to. Therefor it is important for users to log in so they can be granted the right permissions to use in the application. Therefor I want to research a way to create a secure log in where user credentials are kept safe from non-authorized people.

## How
To execute this research I will make use of the DOT Framework. The DOT Framework consists of 5 research strategies.

![Library](https://ictresearchmethods.nl/images/thumb/8/87/Logo-library.png/50px-Logo-library.png)

Library research is done to explore what is already done and what guidelines and theories exist that could help you further your design. Since the advent of the internet library research is also called desk research.

![Field](https://ictresearchmethods.nl/images/thumb/d/d4/Logo-field.png/50px-Logo-field.png)

Field research is done to explore the application context. You apply a field strategy to get to know your end users, their needs, desires and limitations as organizational and physical contexts in which they will use your product.

![Lab](https://ictresearchmethods.nl/images/thumb/a/ac/Logo-lab.png/50px-Logo-lab.png)

Lab research is done to test parts or concepts of your product, of the final product. You use lab research to learn if things work out the way you intended them, or to test different scenarios.

![Showroom](https://ictresearchmethods.nl/images/thumb/2/22/Logo-showroom.png/50px-Logo-showroom.png)

Showroom research is done to test your ideas in relation to existing work. Showing your prototype to experts can be a form of showroom research or spelling out how your product is different from the competition. Also testing your product to general guidelines is a form of showroom research.

![Workshop](https://ictresearchmethods.nl/images/thumb/e/ea/Logo-workshop.png/50px-Logo-workshop.png)

Workshop research is done to explore opportunities. Prototyping, designing and co-creation activities are all ways to gain insights in what is possible and how things could work.

For my research I will be using 2 of the strategies, Library and Workshop research.

## Research Questions

### Create authentication my self or use a authentication framework
The first consideration of creating authentication for my IP is, do I create it myself or do I make use of existing authentication frameworks. If I would create the authentication myself I would have to take a lot of security issues in mind. According to research there are 11 common vulnerabilities when is comes to authentication. These are:
1. **Flawed Brute-Force Protection:** A brute-force attack, such as a dictionary attack, is an attempt to gain illegal access to a system or user’s account by entering large numbers of randomly generated or pregenerated combinations of usernames and passwords until they find one that works. If there’s a flawed brute-force protection system such as a flaw in the authentication logic, firewall, or secure shell (SSH) protocol, attackers can hijack login credentials and processes, compromising the security of user credentials.
2. **Weak Login Credentials:** When users register for an account on a site or application that uses password-based logins, they’re prompted to create a username and password. However, if the password is predictable, this can lead to vulnerabilities in the authentication process. Predictable usernames can make it easier for attackers to target specific users. Rather than using a full brute-force attack, the attackers will look for accounts with easy-to-guess passwords, which are used far too often. They’ll try common credentials like "admin," "admin1," and "password1." With no restrictions on weak passwords, even sites protected against brute-force attacks can find themselves compromised.
3. **Username Enumeration:** Username enumeration is not exactly an authentication vulnerability. But, it can make an attacker’s life easier by lowering the cost for other attacks, such as brute-force attacks or weak credential checks. The problem with username enumeration is that attackers can tell what usernames are valid. Then, they can try to hack valid user accounts using brute-force techniques without wasting their time and money testing a multitude of invalid account names.
4. **HTTP Basic Authentication:** This classic web authentication protocol is easy to implement, however, it is not without its risks. HTTP basic authentication is simple, sending a username and password with each request. However, if appropriate security protocols such as TLS session encryption are not used for all communication, the username and password information can be sent in the clear, making it easy for attackers to steal the credentials.
5. **Poor Session Management:** A vulnerability in the management of session identifiers leads to hijacking of valid authenticated sessions. This is one of the common web vulnerabilities to bypass passwords. There are several session mismanagement vulnerabilities such as no session timeouts, exposure of session IDs in URLs, session cookies without the Http-Only flag set, and poor session invalidation. If attackers can seize control of an existing session, they easily get into a system by assuming the identity of an already-authenticated user, bypassing the authentication process entirely. 
6. **Staying Logged In:** A "Remember me" or "Keep me logged in" checkbox beneath a login form makes it super easy to stay logged in after closing a session. It generates a cookie that lets you skip the process of logging in. However, this can lead to a cookie-based authentication vulnerability if an attacker can predict a cookie or deduce its generation pattern. They can use malicious techniques like brute-force attacks to predict cookies, and cross-site scripting (XSS) to hack user accounts by allowing a malicious server to make use of a legitimate cookie.
7. **SQL Injection:** SQL injection is an attack vector that uses malicious SQL code input in an unexpected way to manipulate and access a database. SQL injections can enable attacks on authentication mechanisms by stealing relevant data (such as poorly protected password hashes) from an unprotected database. They can also bypass authentication mechanisms if the injected SQL code is executed by an internal tool that failed to sufficiently validate external input.
8. **Unsecure Password Change and Recovery:** Sometimes, users forget or just want to change their passwords and click the "Forgot password" or "Lost your password" links. The password reset process poses an authentication vulnerability if an application uses a weak password recovery mechanism such as easy security questions, no CAPTCHAs, or password reset e-mails with overly long or no timeouts. If the password recovery functionality is flawed, attackers can potentially use brute-force techniques or access to other compromised accounts to gain access to user accounts and credentials that are well-protected under normal circumstances.
9. **Flawed Two-Factor Authentication:** While two-factor authentication (2FA) is effective for secure authentication, it can cause critical security issues if not well-implemented. Attackers can figure out the four- and six-digit 2FA verification codes through SIM swap attacks if they are sent through SMS. Some two-factor authentication is also not truly two-factor; if a user is attempting to access sensitive information on a stolen phone using cached credentials, a "second factor" that sends a message to that same phone adds no additional security. Two-factor authentication vulnerabilities can also occur if there’s no brute-force protection to lockout an account after a specific number of attempted logins.
10. **Vulnerable Authentication Logic:** Logic vulnerabilities are common in software applications. This occurs as a result of poor coding or design that affects authentication and authorization access, and application functionality. Flawed application logic can be due to the abuse of functionality, weak security measures, or a skipped step in the verification procedure. For example, an application can prompt a user to answer a security question the logic deems as something "only the correct person would know." But questions like the user’s birthday or mother’s maiden name are often easy to discover. This vulnerability makes it easy for cyber attackers to bypass authentication and gain illegal access to such accounts.
11. **Human Negligence:** According to Shred-it 2020 report, up to 31% of C-suite executives reported employee negligence to be the second major cause of their data breaches. Human error can result in serious authentication vulnerabilities that are far easier to take advantage of than brute-force attacks, SQL injections, and authentication bypasses. This negligence includes actions such as:
    - Leaving a computer on and unlocked in a public place.
    - Losing devices to theft.
    - Leaking sensitive information to strangers.
    - Writing bad code.

#### Conclusion
For my IP I will be using a Authentication framework. The common vulnerabilities have already been tackled by well known frameworks. They are trusted frameworks and there would be no gain in creating the authentication myself, since the frameworks are relatively easy to implement and probably better implemented then I could myself.

### Which frameworks are available for Javascript

## Sources
[The DOT Framework - ICT Research Methods](https://ictresearchmethods.nl/The_DOT_Framework)
[11 Common Authentication Vulnerabilities You Need To Know](https://www.strongdm.com/blog/authentication-vulnerabilities)
