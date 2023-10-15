# Security Concepts
Security is the protection of data, systems, and communications from unauthorized access, damage, or theft. Security is a fundamental concern in the digital age, given the prevalence of cyber threats.

**Computer Security** - 
Generic name for the collection of tools designed to protect data and to thwart hackers 

**Network Security** - 
Measures to protect data during their transmission 

**Internet Security** - 
Measures to protect data during their transmission over a collection of interconnected networks

- Computer System security
- Network security 
- Transport security 
- Wireless security
- Internet security 
- Email security 
- IP security
 

### Need of Security
 - Maintain Privacy
 - Maintain Confidentiality
 - Prevent data loss
 - Prevent from cyber attacks
 - Data Ownership and control
 - Trust and reputation

**Security approaches** refer to the strategies, methodologies, and principles used to achieve security goals in the context of information technology and data protection. These approaches are employed to address various security challenges and threats. Here are some common security approaches:

 - Security Attack
 - Security Mechanism
 - Security Service

**Security attack** - Any action that compromises the security of information owned by an organization.
**Security mechanism** - A process that is designed to detect, prevent, or recover from a security attack. 
 **Security service** - A processing or communication service that enhances the security of the data processing systems and the information transfers of an organization
 
 ---
 ### **Security Service** 

 - Enhance security of data processing systems and information transfers
   of an organization
 - Intended to counter security attacks
 - Using one or more security mechanisms
 - Often replicates functions normally associated with physical
   documents
   Example: 
	 - have signatures, dates; 
	 - be recorded or license  
	 - need protection from disclosure, tampering, or destruction; 
	 - be notarized or witnessed; 

Security Services (X.800) 
Authentication - assurance that the communicating entity is the one claimed 
Access Control - prevention of the unauthorized use of a resource Data 
Confidentiality –protection of data from unauthorized disclosure 
Data Integrity - assurance that data received is as sent by an authorized entity 
Non-Repudiation - protection against denial by one of the parties in a communication
 
 ### Security Mechanism
 - feature designed to detect, prevent, or recover from a security attack
 - no single mechanism that will support all services required
 - however one particular element underlies many of the security mechanisms in use: cryptographic techniques / cryptographic algorithms
 - Like Security Mechanism (X.800)

This model requires to: 
1. select appropriate gatekeeper functions to identify users (**authentication**) 
2.  implement security controls to ensure only **authorised** users access designated information or resources (**access control**)

![Network Security Model](https://binaryterms.com/wp-content/uploads/2020/05/Network-Security-Model.jpg)

To follow the security model it requires to: 
1. design a suitable algorithm for the security transformation (e.g. encryption)
2. generate the secret information (keys) used by the algorithm (e.g. key generation, key scheduling) 
3. develop methods to distribute and share the secret information (e.g. key distribution algorithms) 
4. specify a protocol enabling the principals to use the transformation and secret information for a security service (e.g. security protocols)

### ATTACK
**Passive Attacks** attempt to learn or make use of information from the system but does not affect system resources. 
- obtain message contents - monitor traffic flows 
- difficult to detect as they do not involve any alteration of the data 
- measures are available to prevent their success

**Active Attacks** attempt to alter system resources or affect their operation. 
- masquerade of one entity as some other 
- replay previous messages 
- modify messages in transit It is quite difficult to prevent active attacks absolutely, 

Because of the wide variety of potential physical, software, and network vulnerabilities. The goal is to detect active attacks and to recover from any disruption or delays caused by them.

---
### Approach 
### 1- Trusted Systems
A trusted system is a computer system that can be trusted to a specified extent to enforce a specified security policy.
a ) It should be tamper-proof. 
b ) It should always be invoked. 
c ) It should be small enough so that it can be tested independently

### 2-Security Model
A. **No Security** In this simplest case, the approach could be a decision to implement no security at all. 
B. Security through **Obscurity** In this model, a system is secure simply because nobody knows about its existence and contents. This approach cannot work for too long, as there are many ways an attacker can come to know about it. 
C. **Host Security** In this scheme, the security for each host is enforced individually. This is a very safe approach, but the trouble is that it cannot scale well. The complexity and diversity of modern sites/organizations makes the task even harder. 
D. **Network Security** Host security is tough to achieve as organizations grow and become more diverse. In this technique, the focus is to control network access to various hosts and their services, rather than individual host security. This is a very efficient and scalable model.

---
### PRINCIPLES OF SECURITY
1.  **Confidentiality:**  
    The degree of confidentiality determines the secrecy of the information. The principle specifies that only the sender and receiver will be able to access the information shared between them. Confidentiality compromises if an unauthorized person is able to access a message.
    
    For example, let us consider sender A wants to share some confidential information with receiver B and the information gets intercepted by the attacker C. Now the confidential information is in the hands of an intruder C.
    
2.  **Authentication:**  
    Authentication is the mechanism to identify the user or system or the entity. It ensures the identity of the person trying to access the information. The authentication is mostly secured by using username and password. The authorized person whose identity is preregistered can prove his/her identity and can access the sensitive information.
    
3.  **Integrity:**  
    Integrity gives the assurance that the information received is exact and accurate. If the content of the message is changed after the sender sends it but before reaching the intended receiver, then it is said that the integrity of the message is lost.

-   **System Integrity:** System Integrity assures that a system performs its intended function in an unimpaired manner, free from deliberate or inadvertent unauthorized manipulation of the system.
-   **Data Integrity:** Data Integrity assures that information (both stored and in transmitted packets) and programs are changed only in a specified and authorized manner.

4.  **Non-Repudiation:**  
Non-repudiation is a mechanism that prevents the denial of the message content sent through a network. In some cases the sender sends the message and later denies it. But the non-repudiation does not allow the sender to refuse the receiver.

**5. Access control:**  
The principle of access control is determined by role management and rule management. Role management determines who should access the data while rule management determines up to what extent one can access the data. The information displayed is dependent on the person who is accessing it.

**6. Availability:**  
The principle of availability states that the resources will be available to authorize party at all times. Information will not be useful if it is not available to be accessed. Systems should have sufficient availability of information to satisfy the user request.  

 **7. Issues of ethics and law**  
The following categories are used to categorize ethical dilemmas in the security system.

Individuals’ right to access personal information is referred to as privacy.  
Property: It is concerned with the information’s owner.  
Accessibility is concerned with an organization’s right to collect information.

Accuracy: It is concerned with the obligation of information authenticity, fidelity, and accuracy.



---



