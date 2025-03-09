# Walkthrough_HackThisSite

# 🛡️ **Penetration Testing Report: Hack This Site Basic Challenges** 🚀

---

## **🧠 Skills Demonstrated**

- **Penetration Testing**
- **Web Application Security**
- **Authentication Bypass**
- **Input Validation & Sanitisation**
- **Command Injection**
- **Encryption Analysis**
- **Cookie Manipulation**
- **Directory Traversal**
- **Security Recommendations & Best Practices**
  
---

## **🔑 Executive Summary**

This report provides a **security assessment** of the Hack This Site Basic Challenges, identifying vulnerabilities present in each level and offering recommendations for securing web applications against similar threats. The vulnerabilities discovered demonstrate common security flaws such as **weak authorisation**, **improper input validation**, and **directory traversal**.

---

## **📋 Scope**

The penetration testing was conducted within the **Hack This Site Basic Challenges**, focusing on discovering vulnerabilities in the web application’s security configurations, authentication mechanisms, and data exposure risks. The assessment does not extend beyond this controlled environment. No external tools were used outside of this environment apart from **web developer tools** within the browser.

---

## **⚖️ Legal Disclaimer**

This penetration testing report is for **educational purposes only** and documents security vulnerabilities identified in the Hack This Site Basic Challenges, a legal and authorised training platform. The tests were conducted within the allowed scope of the Hack This Site environment, and no **unauthorised testing** was performed on real-world or third-party systems. Any use of this information outside of legal and ethical guidelines is strictly prohibited.

---

## **🔍 Vulnerability Descriptions and Key Findings**

### **Level 1: The Idiot Test** 🚫
- **🔒 Vulnerability:** Password visible in HTML source code.
- **💡 Recommendation:** 
  - Avoid storing sensitive data in client-side code.
  - Implement **server-side authorisation**.

---

### **Level 2: Missing Password File** 📂
- **🔒 Vulnerability:** The authentication script references a missing password file, allowing bypass.
- **💡 Recommendation:** 
  - Ensure critical authentication files are uploaded and protected.

---

### **Level 3: Exposed Password File** 🔓
- **🔒 Vulnerability:** Password stored in a publicly accessible PHP file, ‘password.php’.
- **💡 Recommendation:** 
  - Secure sensitive files by restricting direct access and using proper permissions.

---

### **Level 4 & 5: Email-Based Exploitation** 📧
- **🔒 Vulnerability:** Password retrieval email address can be modified by users in browser developer tools.
- **💡 Recommendation:** 
  - Implement proper **input validation** and avoid exposing sensitive logic in client-side code.

---

### **Level 6: Weak Encryption** 🔑
- **🔒 Vulnerability:** Predictable encryption algorithm (Caesar cipher) that can be decrypted manually.
- **💡 Recommendation:** 
  - Use **industry-standard cryptographic methods** and avoid weak custom encryption.

---

### **Level 7 & 8: Command Injection via UNIX Commands** 💻
- **🔒 Vulnerability:** Application accepts user input without proper sanitisation, allowing command injection.
- **💡 Recommendation:** 
  - Validate and sanitise user input before processing commands.

---

### **Level 9: Directory Traversal** 🗂️
- **🔒 Vulnerability:** Misconfigured access control allows navigation to restricted directories.
- **💡 Recommendation:** 
  - Implement strict **access control policies** and prevent directory listing.

---

### **Level 10: Cookie Manipulation** 🍪
- **🔒 Vulnerability:** Authorisation determined via a modifiable cookie within browser developer tools.
- **💡 Recommendation:** 
  - Use **secure session handling** and server-side validation for authorisation.

---

### **Level 11: Misconfigured .htaccess File** 🔐
- **🔒 Vulnerability:** The `.htaccess` file is publicly accessible, exposing security configurations.
- **💡 Recommendation:** 
  - Restrict access to sensitive configuration files and ensure secure server settings.

---

## **💡 Security Recommendations**

1. **🔒 Implement Secure Authorisation:** Store passwords securely using **hashing algorithms**.
2. **🛡️ Input Validation & Sanitisation:** Prevent **command injection** and **XSS** vulnerabilities by validating and sanitising all user inputs.
3. **🔑 Access Control & Directory Protection:** Restrict access to sensitive files and directories to prevent **unauthorised access**.
4. **🔏 Use Secure Encryption Methods:** Replace weak encryption mechanisms with **industry-standard cryptographic solutions**.
5. **🍪 Secure Session Management:** Prevent **cookie manipulation** by implementing secure session handling techniques.
6. **🖥️ Server Hardening:** Disable directory listing, enforce strict **file permissions**, and properly configure **web server security settings**.

---

## **📌 Conclusion**

The vulnerabilities identified in the Hack This Site Basic Challenges demonstrate critical security flaws commonly found in web applications. Implementing the recommended security measures will **mitigate these risks** and strengthen the overall security posture of web applications. 

Organisations should conduct **regular security assessments** and adopt best practices in **secure coding** and **application development**.

---

**Next Steps:**
- 🚀 Continue exploring advanced challenges.
- 🛠️ Collaborate with developers to implement **secure coding practices**.
- 🔄 Monitor and test security regularly to stay ahead of emerging threats.
