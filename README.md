# CS-305-Software-Security

# Artemis Financial – Secure Software Practices Report  
**Developer:** Todd Jarmiolowski  
**Course:** CS 305 – Software Security  

---

## Project Overview  
This repository contains my completed **Artemis Financial Practices for Secure Software Report**, which documents how I implemented secure communications, encryption, and vulnerability testing for a financial services client. The project demonstrates my ability to identify software vulnerabilities, refactor insecure code, and apply industry best practices for secure software development.

---

## Client Summary  
**Client:** Artemis Financial  
**Objective:** Secure communication and data integrity for a Spring Boot web service.  
Artemis Financial requested implementation of modern encryption protocols and secure software practices to protect sensitive financial transactions. The company wanted to integrate HTTPS (TLS 1.3), add a checksum verification feature, and perform a vulnerability assessment using OWASP tools to ensure compliance with current security standards.

---

## Reflection Questions

### 1. What issue did the company want you to address?  
Artemis Financial wanted their application secured for data transmitted between clients and servers. The goal was to implement strong encryption, refactor the existing codebase to support HTTPS, and ensure proper verification of transmitted data through secure hashing and certificate validation.

---

### 2. What did you do well when you found your client’s software security vulnerabilities?  
I successfully identified and mitigated outdated or vulnerable dependencies using **OWASP Dependency-Check**. I implemented **TLS 1.3 with AES-256-GCM encryption** and configured a valid **PKCS#12 keystore**. Secure coding practices ensure the protection of client data, maintain user trust, and protect the organization’s reputation.

---

### 3. Which part of the vulnerability assessment was challenging or helpful to you?  
Interpreting the OWASP Dependency-Check report was challenging but highly educational. It helped me learn how to analyze dependency risks, refactor code safely, and confirm that no critical vulnerabilities remained. It reinforced how vital static analysis tools are in secure software development.

---

### 4. How did you increase layers of security?  
I enforced **TLS 1.3 only**, implemented **AES-256-GCM** encryption, and used **SHA-256** for the checksum verification endpoint. These changes increased both confidentiality and integrity of data in transit. In future projects, I plan to integrate tools like **OWASP ZAP**, **Burp Suite**, and continuous CI/CD vulnerability scanning for automated detection and mitigation.

---

### 5. How did you make certain the code and software application were functional and secure?  
I launched the refactored Spring Boot application in Eclipse and accessed `https://localhost:<port>/hash`. The browser’s lock icon confirmed active TLS encryption. The endpoint correctly displayed the SHA-256 checksum, proving data integrity. I verified no runtime errors and validated the “BUILD SUCCESS” message from **OWASP Dependency-Check**.

---

### 6. What resources, tools, or coding practices did you use that might be helpful in future assignments or tasks?  
I used **Eclipse**, **Spring Boot**, **TLS 1.3**, **SHA-256**, and **OWASP Dependency-Check**. I followed **NIST** and **OWASP** standards to secure communications and harden application code. These tools and practices will guide my approach to secure coding, encryption, and vulnerability testing in future software projects.

---

### 7. What might you show future employers from this assignment?  
This project demonstrates my ability to apply industry-standard security controls such as encryption, certificate management, and vulnerability scanning. It shows hands-on experience securing a Java web service using modern cryptographic protocols, following secure software development life-cycle (SSDLC) practices, and understanding secure deployment principles.

---

## Repository Contents  
- `CS 305 Project Two Report.docx` – Completed Artemis Financial Secure Software Report  
- Screenshots for certificate generation, checksum verification, HTTPS operation, dependency-check, and functional testing  
- `README.md` – Reflection responses and project overview  

---

## Tools and Standards Used  
- **Programming:** Java (Spring Boot)  
- **IDE:** Eclipse  
- **Encryption:** TLS 1.3, AES-256-GCM, SHA-256  
- **Testing:** OWASP Dependency-Check, browser HTTPS validation  
- **Standards Followed:** OWASP Top 10, CIS Controls, NIST SP 800-53  

---


