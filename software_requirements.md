### **The Chronicles of Software Requirements**

In a realm of endless innovation, a group of software developers embarked on a legendary quest to build a perfect system. Their mentor, an experienced guide, welcomed them into the world of **software requirements** and explained, *“Before you can create, you must first understand. Requirements are the foundation of your journey.”*

---

### **Act 1: The Origin of Requirements**

The mentor began, “A **requirement** is the key to understanding what the system must do and how it should operate. It can range from a high-level abstract idea to a detailed mathematical specification. But beware! Requirements serve a dual purpose:
1. They help you win contracts by describing what the system will achieve.
2. They hold you accountable by specifying what must be delivered.”

---

### **Act 2: The Two Pillars – User and System Requirements**

The team encountered the two central pillars of requirements:

#### **1. User Requirements**
- These are high-level statements written in **natural language** and diagrams.
- Their purpose? To help customers understand the system’s goals.

#### **2. System Requirements**
- These are structured, detailed documents that describe **what needs to be implemented**.
- They serve as a bridge between the developers and the customer, often forming part of the contract.

The mentor explained through an example:
- **User Requirement**: “The software must provide a means of accessing external files.”
- **System Requirement**: “External files must be represented by icons, and users should be able to define, select, and apply tools to these files.”

“Remember,” the mentor said, “User requirements are for dreams, while system requirements are for reality.”

---

### **Act 3: The Three Types of Requirements**

The developers soon learned of the three types of requirements, each vital to the quest:

#### **1. Functional Requirements**
These describe:
- **What the system should do**.
- **How it reacts** to specific inputs and situations.

**Example (Library System)**:
1. Users must be able to search databases or a subset.
2. The system should provide viewers for reading documents.
3. Each order must have a unique identifier.

#### **2. Non-Functional Requirements**
“These requirements,” the mentor warned, “are just as important as functional ones. If they fail, the system is worthless.”

Non-functional requirements represent **qualities of the system**, including:
- **For users**: Performance, usability, reliability.
- **For developers**: Portability, maintainability.
- **For owners**: Cost and benefits.

**Examples**:
1. **Product**: The interface must use HTML, avoiding Java applets.
2. **Organizational**: Development must follow XYZCo-SP-STAN-95 standards.
3. **External**: Customer data must remain confidential, revealing only names and reference numbers.

#### **3. Domain Requirements**
“These are drawn from the system’s domain,” the mentor explained. “They reflect the unique environment in which the system operates.”

**Example (Library System)**:
- Copyright laws dictate that certain documents must be deleted upon arrival.

---

### **Act 4: Challenges of the Journey**

The developers faced numerous challenges as they tried to capture these requirements:

1. **Imprecision**:
   Ambiguous terms, such as “appropriate viewers,” led to confusion. Developers and users often interpreted them differently.

2. **Completeness and Consistency**:
   Requirements should describe everything the system needs (**complete**) and avoid contradictions (**consistent**). However, achieving both was rarely possible.

3. **Conflicts in Requirements**:
   For example:
   - In a spacecraft system, reducing the number of chips minimized weight.
   - But using low-power chips required more chips, creating a conflict.
   The developers had to prioritize which requirement mattered most.

---

### **Act 5: Gathering the Knowledge**

To overcome these challenges, the team used various methods to gather and analyze requirements:

#### **1. Observation**
They shadowed users, watching and learning from their daily tasks.

#### **2. Interviews**
They conducted sessions to ask users:
- What do you need?
- What challenges do you face?
- What is your vision for the future?

#### **3. Brainstorming**
In group sessions, they explored ideas with a moderator guiding discussions.

#### **4. Prototyping**
They created:
- **Paper prototypes**: Simple sketches of screens.
- **Mockups**: Functional interfaces to simulate the system.

#### **5. Use Case Analysis**
They analyzed:
- **Actors**: Users or systems interacting with the software.
- **Use Cases**: Scenarios describing how the system would be used.

**Example (ATM System)**:
- **Actors**: User, ATM, Bank.
- **Use Case**: “Withdraw Cash.”
   - **Pre-condition**: User is logged in.
   - **Successful Path**: The system retrieves the balance, validates the withdrawal amount, and disperses cash.

---

### **Act 6: Recording the Requirements**

With their findings in hand, the developers needed a way to document their requirements clearly. They used:

#### **1. Natural Language**
- Flexible but prone to ambiguity.

#### **2. Structured Language**
- Templates ensured clarity and uniformity.

#### **3. Form-Based Specifications**
- Each function was described with:
  - Inputs, outputs, pre-conditions, post-conditions, and side effects.

**Example (Insulin Pump)**:
- **Function**: Compute insulin dose.
- **Input**: Current and past sugar levels.
- **Output**: Dose to be administered.
- **Side Effects**: None.

#### **4. Tabular Specifications**
- Tables helped represent multiple conditions and outcomes.

**Example**:
| Condition                              | Action                     |
|----------------------------------------|----------------------------|
| Sugar level falling                    | Dose = 0                  |
| Sugar level stable                     | Dose = 0                  |
| Sugar level increasing steadily        | Dose = (ΔSugar)/4         |

#### **5. Graphical Models**
- Diagrams visually depicted processes and relationships.

---

### **Act 7: The Requirements Document**

Finally, the developers compiled everything into a **requirements document**, a sacred text that would guide the system’s creation. It included:
1. Functional and non-functional requirements.
2. User and system requirements.

The document followed the **IEEE Standard**, which structured it into:
1. Introduction.
2. General Description.
3. Specific Requirements.
4. Appendices.
5. Index.

The mentor emphasized, “This document is not about how the system works—it’s about what the system should do.”

---

### **Act 8: The Key Takeaways**

As their journey neared completion, the developers reflected on what they had learned:
1. Requirements define what the system must do and the constraints on its operation.
2. **Functional requirements** describe the system’s behavior, while **non-functional requirements** define its qualities.
3. Requirements must be clear, consistent, and complete.
4. A well-structured **requirements document** is essential for success.

---

### **Epilogue: A Legacy of Requirements**

With their requirements defined, the developers began building their system. They knew their journey was far from over, but their foundation was strong. Their story became a guiding light for others embarking on the same quest, proving that a solid understanding of requirements could turn dreams into reality.

---

Here’s a list of **possible questions** based on the slides, along with their **answers** to help you prepare for the exam:

---

### **Basic Concepts of Requirements**

1. **Q: What is requirements engineering?**
   - **A:** Requirements engineering is the process of establishing the services a system must provide and the constraints under which it operates and is developed.

2. **Q: What is a requirement?**
   - **A:** A requirement is a description of a system service or constraint. It can range from a high-level abstract statement to a detailed technical specification.

3. **Q: What are the dual purposes of requirements?**
   - **A:** Requirements can:
     1. Serve as the basis for a contract (open to interpretation).
     2. Be a binding document for implementation (defined in detail).

---

### **Types of Requirements**

4. **Q: What are the types of requirements?**
   - **A:** 
     1. **User Requirements**: High-level descriptions written in natural language with diagrams, targeted at customers.
     2. **System Requirements**: Detailed technical specifications defining system functionality and constraints for developers.
     3. **Domain Requirements**: Requirements specific to the system’s domain, reflecting characteristics or constraints of that domain.

5. **Q: What is the difference between user and system requirements?**
   - **A:** 
     - **User Requirements**: Written for customers, describing what the system should do in plain language.
     - **System Requirements**: Technical documents for developers, detailing how the system will achieve the user requirements.

---

### **Functional, Non-Functional, and Domain Requirements**

6. **Q: What are functional requirements?**
   - **A:** Functional requirements describe the services the system should provide, how it should react to specific inputs, and its behavior in certain situations.

7. **Q: What are non-functional requirements?**
   - **A:** Non-functional requirements define system attributes such as performance, usability, reliability, and constraints like cost or standards compliance.

8. **Q: Why are non-functional requirements critical?**
   - **A:** Non-functional requirements often determine the system's usability and success. If they are not met, the system may fail entirely.

9. **Q: What are domain requirements?**
   - **A:** Domain requirements are derived from the application’s domain and include system-specific characteristics or constraints.

10. **Q: Give an example of a domain requirement.**
    - **A:** In a library system, copyright restrictions may require some documents to be deleted immediately upon arrival.

---

### **Challenges in Requirements Engineering**

11. **Q: What challenges are faced in requirements engineering?**
    - **A:** 
      1. **Imprecision**: Ambiguous requirements can lead to different interpretations.
      2. **Completeness**: Ensuring all requirements are included is difficult.
      3. **Consistency**: Avoiding contradictions in requirements is challenging.
      4. **Conflicts**: Conflicting requirements, such as minimizing weight vs. power consumption in spacecraft systems.

12. **Q: Why is ambiguity in requirements problematic?**
    - **A:** Ambiguity causes misunderstandings between users and developers, leading to incorrect implementations.

---

### **Requirement Gathering Techniques**

13. **Q: What are the techniques for gathering requirements?**
    - **A:** 
      1. Observation
      2. Interviews
      3. Brainstorming
      4. Prototyping (paper or mockup)
      5. Use case analysis

14. **Q: What is a use case?**
    - **A:** A use case specifies a sequence of actions performed by a system, subsystem, or class in interaction with external actors.

15. **Q: What are the components of a use case?**
    - **A:** 
      - Name
      - Description
      - Actors
      - Pre-conditions
      - Post-conditions
      - Successful path
      - Alternative path
      - Rules and exceptions

---

### **Writing Requirements**

16. **Q: What are some formats for writing requirements?**
    - **A:** 
      1. **Natural Language**: Flexible but prone to ambiguity.
      2. **Structured Language**: Templates to ensure uniformity.
      3. **Form-Based Specifications**: Includes inputs, outputs, pre-conditions, and side effects.
      4. **Tabular Formats**: Useful for representing alternative scenarios.
      5. **Graphical Models**: Diagrams for visual representation.

17. **Q: What is a form-based specification?**
    - **A:** A structured way of documenting requirements by specifying inputs, outputs, pre-conditions, post-conditions, and side effects.

18. **Q: What is the advantage of graphical models?**
    - **A:** Graphical models help visualize sequences, actions, and state changes, making complex processes easier to understand.

---

### **The Requirements Document**

19. **Q: What is a requirements document?**
    - **A:** The requirements document is the official statement of what is required of the system developers. It defines what the system should do (functional requirements) and the constraints it must follow (non-functional requirements).

20. **Q: What are the sections of a requirements document?**
    - **A:** 
      1. Introduction
      2. General Description
      3. Specific Requirements
      4. Appendices
      5. Index

21. **Q: What is the IEEE standard structure for requirements?**
    - **A:** The IEEE standard provides a generic structure that includes:
      - Introduction
      - General Description
      - Specific Requirements
      - Appendices
      - Index

22. **Q: Why is a requirements document important?**
    - **A:** It serves as an agreed-upon reference for developers and stakeholders, ensuring the system meets its intended goals.

---

### **Key Concepts for Requirements**

23. **Q: What are key points to remember about requirements?**
    - **A:** 
      1. Requirements set out what the system should do and its constraints.
      2. Functional requirements describe services the system provides.
      3. Non-functional requirements constrain the system or its development process.
      4. User requirements should be simple and written in natural language.
      5. System requirements should be precise and technical.

24. **Q: Why must requirements focus on “what” and not “how”?**
    - **A:** Requirements should describe **what the system needs to achieve**, leaving implementation details to the design phase.

---

### **Advanced Questions**

25. **Q: How can requirements be verified?**
    - **A:** Non-functional requirements must be quantifiable (e.g., “response time < 1 second for 95% of transactions”) to allow objective testing.

26. **Q: What are some common problems with requirements documents?**
    - **A:** 
      - Lack of clarity.
      - Mixing functional and non-functional requirements.
      - Combining multiple requirements into a single statement.

27. **Q: How do requirements interact in complex systems?**
    - **A:** Non-functional requirements often conflict, requiring prioritization based on system goals.

28. **Q: How does use-case analysis help in functional requirements?**
    - **A:** Use-case analysis identifies:
      - Actors
      - Tasks
      - Interaction scenarios, ensuring the system meets user needs.

---
