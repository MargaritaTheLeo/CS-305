# CS-305

**Artemis Financial Practices for Secure Software Report**

The client for this project, Artemis Financial, is a company that specializes in developing financial plans for their customers. When creating the plans, the company takes into consideration their client’s needs and expectations implementing an individualized approach to each of them. Artemis Financial offers development of savings, investments, retirement, and insurance plans. 

Striving to provide the best service to their clients, Artemis Financial is looking to make their current operations more modern and up to date with the software security requirements. Given that Artemis Financial values their clients’ privacy and the security of their personal data, the company is seeking assistance in protecting their clients and the organization itself from various security threats.

My role in this project was to conduct a thorough exam of the web-based software application of Artemis Financial in order to identify security vulnerabilities. During the examination, I was expected to thoroughly document all our findings in this vulnerability assessment report. Thereafter, this report was used to mitigate Artemis Financial software vulnerabilities.  

One essential component of software development is secure coding. It describes the process of developing code that is impervious to hacking, illegal access, and other security risks. Secure coding has several advantages, such as better application security, a lower chance of data breaches, and a rise in client confidence.

Secure coding helps improve overall application security by reducing the risk of vulnerabilities that can be exploited by attackers. Developers may avoid common security flaws like buffer overflows, SQL injection, and cross-site scripting (XSS) by adhering to safe code principles. Attackers may use these flaws to take over the program, alter or remove data, or obtain unauthorized access to private information.

Data breaches can have serious consequences for businesses, including loss of revenue, reputational damage, and legal liabilities. By avoiding flaws that attackers may exploit, secure coding can significantly lower the risk of data breaches. Developers can lessen the possibility of illegal access to sensitive data, including financial information, intellectual property, and personal information, by putting safe coding principles into effect.

In today's digital age, customers are increasingly concerned about the security of their data. By implementing secure coding practices, developers can demonstrate their commitment to privacy and data security. This can help build customer trust and loyalty, which can ultimately lead to increased sales and revenue.
I started my project with a manual review of the provided code. This review revealed that the code did not utilize neither encryption nor error handling mechanisms. Lack of encryption always leads to a possibility of data theft because the data is not protected during its storage and transmission. Additionally, lack of error handling can potentially cause unexpected errors and security hazards. 
The provided code also did not have any input validation mechanisms. I decided to implement input validation for the prevention of malicious injection attacks. Doing so helps us handle input sanitization, preventing SQL injection threats.

The cipher I chose for this project was SHA-256. This algorithm converts the information into a 256-bit code consisting of 64 letters or digits composed randomly. As a result, almost unique combinations are generated, which are extremely difficult to decipher. The reverse conversion is impossible, which makes SHA-256 one of the most secure algorithms. This cipher mechanism has been continuously proving itself to be secure and relatively simple to implement. Additionally, because of the way SHA-256 works, it has a very low chance of collisions, which is important to our client.

Once I ran Maven Dependency Check, I was able to see a list of all code dependencies and vulnerabilities. After having done so, I eliminated false positives from the report. A false positive is basically a vulnerability erroneously identified by the dependency-check tool. Hence, the false positive is a software vulnerability that in actuality does not exist. By eliminating false positives, we can make sure that the time dedicated to improving application’s safety is spent wisely and efficiently. 

When working on this project, I made sure I followed the standards of secure coding. Secure coding is basically a set of practices that ensures the security of software applications. Secure coding involves identifying potential security vulnerabilities and addressing them during the application development process. It also includes implementing security controls to protect against malicious attacks. Best practices for secure coding are the following: shift-left security, embedded security, use of resources such as OWASP, implementation of static and dynamic application security tools, software composition analysis, and compliance with standards and regulatory requirements. 

Secure coding is important because it helps prevent cyber-attacks and data breaches. Cyberattacks can cause significant damage to an organization, including financial loss, reputational damage, and legal liabilities. Secure coding can help prevent these types of attacks by creating software that is resistant to vulnerabilities and malicious attacks.



