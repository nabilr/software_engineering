
### **1. Introduction to Software Requirements**
   - **Objectives**
     - Understand user and system requirements.
     - Learn about functional and non-functional requirements.
     - Explore how to organize requirements in a requirements document.
     - **Example**: For a banking app, the system must be user-friendly while supporting secure transactions.

   - **Topics Covered**
     - Functional and Non-Functional Requirements
     - User and System Requirements
     - Interface Specification
     - Requirements Documentation

---

### **2. Foundations of Requirements Engineering**
   - **Requirements Engineering Process**
     - Define services that the user needs.
     - Identify constraints within which the system operates.
     - **Example**: For an online shopping platform, services include browsing and checkout, while constraints may be server capacity and data protection laws.

   - **What is a Requirement?**
     - Requirements can range from high-level statements to detailed technical specifications.
     - Serve dual purposes:
       1. Basis for contracts between client and developer.
       2. Framework for system design and implementation.
     - **Example**: “The system should be user-friendly” (high-level) vs. “The system must include a search bar on every page” (detailed).

---

### **3. Types of Requirements**
   - **User Requirements**
     - General statements describing what the user expects from the system.
     - Written in simple language, often without technical jargon.
     - **Example**: "The software should allow file uploads."

   - **System Requirements**
     - Detailed technical descriptions of what the system must do.
     - Defines the exact functionalities to be implemented.
     - **Example**: "Users shall be able to upload files up to 20 MB in size, with support for .pdf, .docx, and .jpeg formats."

   - **User vs. System Requirements: An Example**
     - **User Requirement**: "The system must provide a way to manage external files."
     - **System Requirement**: "The system shall display each external file type as a specific icon, which the user can click to open."
     - **Example**: For a photo management app, a user requirement might be "Organize photos," while system requirements specify how they’re sorted, filtered, and displayed.

---

### **4. Types of Software Requirements**
   - **Functional Requirements**
     - Define what the system must do, such as specific tasks, inputs, and outputs.
     - **Example**: In a library system, "The user shall be able to search for books by title, author, or genre."

   - **Non-Functional Requirements**
     - Constraints on system performance, usability, and quality.
     - Often define the system’s quality attributes.
     - **Example**: "The system must have a downtime of less than 1 hour per year."

   - **Domain Requirements**
     - Derived from the specific field or domain the system is in.
     - Can add new functionalities or constraints on existing requirements.
     - **Example**: In a healthcare system, domain requirements could specify that patient data must be encrypted.

---

### **5. Understanding Functional Requirements**
   - **Definition of Functional Requirements**
     - Describe the services the system is expected to provide.
     - Define the behavior based on inputs and outputs.
     - **Example**: In a hotel booking system, a functional requirement might be "Allow users to search for hotels by city and dates."

   - **The LIBSYS System**
     - A hypothetical library system example.
     - Provides users with access to a range of databases for personal study.
     - **Functional Requirements for LIBSYS**:
       - Users can search across multiple databases or a subset.
       - Document viewers must be available for reading stored articles.

---

### **6. Challenges in Defining Requirements**
   - **Requirements Imprecision**
     - Ambiguity in requirements can lead to misunderstandings.
     - **Example**: "Appropriate viewers" might be interpreted differently by the user (specialized viewer per document) versus the developer (generic text viewer).

   - **Completeness and Consistency**
     - Ideally, requirements should cover all necessary aspects and be free from contradictions.
     - **Example**: If an app is required to work on iOS and Android, no feature should be exclusive to just one platform.

---

### **7. Exploring Non-Functional Requirements**
   - **Definition and Importance**
     - Define quality aspects like performance, security, and usability.
     - Non-functional requirements can be more crucial than functional ones.
     - **Example**: In a food delivery app, it may state, "Pages must load within two seconds under standard internet speeds."

   - **Types of Non-Functional Requirements**
     - **Product Requirements**: Specific constraints on the product itself.
       - **Example**: "The UI shall use simple HTML without frames or Java applets."
     - **Organizational Requirements**: Standards and guidelines imposed by the organization.
       - **Example**: "The system must adhere to ISO 9001 standards."
     - **External Requirements**: Legal or ethical constraints.
       - **Example**: "The system shall comply with HIPAA to protect patient information."

---

### **8. Crafting and Validating Non-Functional Requirements**
   - **Goals and Requirements**
     - Goals provide general intentions, while verifiable requirements allow objective measurement.
     - **Example**:
       - **Goal**: "The system should be easy to use."
       - **Verifiable Requirement**: "Users shall be able to complete all system functions after two hours of training."

   - **Writing Quantifiable Requirements**
     - Non-functional requirements should be measurable.
     - **Example**: "An operator shall not have to wait more than 1 second for a transaction to complete in 95% of cases."

---

### **9. Techniques for Gathering Requirements**
   - **Observation and Interviews**
     - Observe users, conduct interviews, and ask about specific needs, future visions, and potential alternatives.
     - **Example**: For a hospital management system, interviewing doctors could reveal needs for features like quick access to patient records.

   - **Prototyping**
     - Create paper or software prototypes to visualize system functionality and gather feedback.
     - **Example**: A paper prototype for a mobile app where each screen is drawn and shown to users to gather input on layout and functionality.

---

### **10. Structuring and Documenting Requirements**
   - **Hierarchy of Requirements Documentation**
     - Requirements documents are usually organized into a hierarchy, starting from broad definitions to specific details.
     - **Example**:
       - **Requirements Definition**: Broad, user-oriented goals.
       - **Requirements Specification**: Detailed, technical requirements for implementation.

   - **Alternatives to Natural Language Specifications**
     - **Structured Natural Language**: Uses standard forms to organize requirements.
     - **Graphical Notations**: Use diagrams, like use cases or sequence diagrams, to represent requirements visually.
     - **Mathematical Specifications**: Based on formal, mathematical concepts for clarity and precision.
       - **Example**: Finite state machines for modeling system states.

   - **Form-Based Specifications**
     - Use predefined forms to maintain a consistent structure.
     - **Example**: In a form-based specification for an insulin pump, inputs and outputs are clearly defined along with pre- and post-conditions.

   - **Tabular Specifications**
     - Useful for detailing multiple possible actions based on conditions.
     - **Example**: For a medical device, conditions like “stable blood sugar” might lead to one action, while “rising blood sugar” leads to another.

---

### **11. Using Graphical Models and Use Case Analysis**
   - **Graphical Models**
     - Helpful for visualizing how the system should change states or perform actions in sequence.
     - **Example**: A sequence diagram showing the steps of withdrawing cash from an ATM.

   - **Use Case Analysis**
     - Defines system actions through interactions with external actors.
     - **Example**: For an ATM, the use cases could include “Withdraw Cash,” “Check Balance,” and “Deposit Cash,” each specifying actions and actors involved.

   - **Pre- and Post-Conditions**
     - Conditions that must be met before and after executing a use case.
     - **Example**: The use case “Order from Catalogue” might have a pre-condition of “User is connected” and a post-condition of “Order record updated.”

---
### **12. Use Case Analysis**
   - **Definition and Purpose**
     - Use cases define interactions between the system and external actors, capturing system functionality from the user's perspective.
     - **Example**: In an ATM system, the use cases could include “Withdraw Cash,” “Check Balance,” and “Deposit Cash.”

   - **Components of a Use Case**
     - **Actors**: Entities (usually people or other systems) interacting with the system.
     - **Initiator**: The primary actor who triggers the use case.
     - **Description**: Overview of the use case scenario and its flow of events.
     - **Pre-Conditions and Post-Conditions**: Requirements before and after the use case is executed.
     - **Example**:
       - **Use Case**: "Withdraw Cash"
       - **Actors**: User, ATM
       - **Pre-Condition**: User must be authenticated.
       - **Post-Condition**: Cash is dispensed, and the account balance is updated.

---

### **13. ATM Use Case Example**
   - **ATM Functions and Use Cases**
     - **Login**: User enters a PIN to access account features.
     - **Withdraw Cash**: User selects an account, enters an amount, and receives cash if funds are available.
     - **Check Balance**: User can view their current account balance.
     - **Transfer

 Funds**: User can transfer money between accounts.
     - **Deposit Cash**: User can add funds to their account via cash deposit.
     - **Example**:
       - **Withdraw Cash**:
         - **Steps**:
           1. User requests cash withdrawal.
           2. ATM validates available funds.
           3. If funds are sufficient, ATM dispenses cash and updates the balance.
         - **Alternate Path**: If funds are insufficient, ATM displays an error message.



---

### **14. Requirements Documentation Standards**
   - **Requirements Document**
     - The formal statement of system requirements, focusing on what the system should do rather than how it will do it.
     - **Example**: It may include sections on the problem, background information, and specific functional and non-functional requirements.

   - **IEEE Requirements Standard**
     - Provides a structured format:
       - **Introduction**: Overview and purpose.
       - **General Description**: Scope and context.
       - **Specific Requirements**: Detailed requirements, both functional and non-functional.
       - **Appendices and Index**: Additional supporting information.
     - **Example**: The IEEE standard is widely adopted to ensure consistency and completeness in requirements documents.

---

Let me know if you need further elaboration on any specific section or topic!
