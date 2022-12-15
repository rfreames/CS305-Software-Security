# CS305-Software-Security

**On Project Two:**

**•	Briefly summarize your client, Artemis Financial, and their software requirements. Who was the client? What issue did they want you to address?**

Artemis Financial is a consulting company which creates financial plans for their customers. These plans include retirement, savings, investment, and insurance. The company wanted me to start the process of adding file verification using a checksum.

**•	What did you do very well when you found your client’s software security vulnerabilities? Why is it important to code securely? What value does software security add to a company’s overall wellbeing?**

The project provided was fairly empty, but I ran a dependency check to determine if there were any vulnerabilities within the given project. I also determined a proper algorithm to use in both certificate generation and checksum verification.

It’s important to code securely as this helps protect a company’s vital information, and by extension, private customer information. By following secure software principles, a company reduces the likelihood of a data breach, loss of information, resources, or otherwise. Keeping information confidential prevents competitors from gaining access to internal operations or products, and improves customer confidence in the company.

**•	What part of the vulnerability assessment was challenging or helpful to you?**

Determining the correct encryption to use in generating a checksum or certificate was a helpful part of the assessment, as it gave me a greater insight into commonly used algorithms, including those recommended by NIST.

**•	How did you increase layers of security? In the future, what would you use to assess vulnerabilities and decide which mitigation techniques to use?**

There were two ways I increased layers of security. First, I generated a certificate to be used in validating the website using the Java Keytool. I also implemented an asymmetric encryption algorithm using SHA-256 to be used in checksum verification. In addition to these, I implemented the use of the certificate through the use of HTTPS, so that when the site is accessed the generated certificate is used. Moving forward I would likely still use online resources from reputable sources such as NIST, OWASP, or other well-known companies. Following industry standards is likely one of the better ways to ensure that software is secure.

**•	How did you make certain the code and software application were functional and secure? After refactoring the code, how did you check to see whether you introduced new vulnerabilities?**

To make sure that the certificate and checksum were correctly implemented, I ran the program and accessed it using localhost on my computer. Once I had access, I verified that HTTPS was being used, the certificate I generated was properly being displayed, and verified that a checksum digit was displayed. In order to make sure I did not introduce additional vulnerabilities, I ran a dependency check to scan for vulnerabilities both prior to and after refactoring code.

**•	What resources, tools, or coding practices did you use that might be helpful in future assignments or tasks?**

A few of the tools I used were the Java Keytool and Maven Dependency Check. I also accessed NIST to review dependencies as well as encryption standards recommended by the US government.

**•	Employers sometimes ask for examples of work that you have successfully completed to show your skills, knowledge, and experience. What might you show future employers from this assignment?**

This project would be good to show a basic level of understanding in implementing encryption algorithms to accomplish various tasks, such as a checksum, certificate generation, or even encryption of data. It would also show a basic understanding of the use of dependencies, as well as reviewing and editing a pom.xml file, implementing a suppression file, and keeping various dependencies up-to-date. Beyond this, the code review section would show an awareness of some simpler aspects of software security, such as the use of input validation, attribute-based access control, and encapsulation.
