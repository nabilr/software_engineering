### **The Architect’s Journey: A Tale of Building a System**

Once upon a time, in the bustling town of Techville, an ambitious architect named Alex was given an exciting challenge: to design a revolutionary system for an online shopping platform. This wasn’t just any system—it had to be intuitive, scalable, and ready for the unexpected twists of real-world users.

---

#### **Act 1: The Characters Take the Stage**

Before Alex could start sketching the blueprint, they knew one thing: every great story needs compelling characters. In the world of systems, these are called **actors**.

- **Primary actors** are the heroes—the users with clear goals. For Alex, the primary actor was the **shopper**, who wanted to find items, add them to a cart, and place orders.
- **Secondary actors** are the supporting cast. These include systems or roles that help the heroes achieve their goals, like the **payment gateway** or **inventory database**.

Alex made a list of all the characters and their roles. This was the foundation of the story.

---

#### **Act 2: Mapping the Story with Use Cases**

With the actors ready, Alex began weaving the story through **use cases**—the individual scenes where the actors interact with the system to achieve their goals.

For example:
1. **Search for Items**: The shopper looks for a product.
2. **Add to Cart**: The shopper selects an item to purchase.
3. **Place Order**: The shopper completes the purchase.

Each use case was named clearly, using **verb-object format** like "Place Order," focusing on the shopper’s perspective. Alex avoided dull, system-centric names like "Payment Processing" because this wasn’t a story about the system—it was about the shopper.

---

#### **Act 3: Building Depth with Relationships**

Alex knew that not all parts of the story could stand alone. Some scenes needed to reuse others, some had optional extensions, and others required a parent-child structure. This is where the relationships came in.

1. **Include: The Reusable Scene**
   - Alex realized that every use case required the shopper to log in. Instead of repeating this sequence, Alex created a separate use case called **Log In**.
   - Now, "Log In" was **included** in other use cases like "Search for Items" and "Place Order." It was a shared subplot, much like a character making recurring appearances in different chapters.

   *For example:*
   - Use Case: **Place Order**
     - Step 1: Include **Log In**.
     - Step 2: Add items to the cart.
     - Step 3: Confirm payment.

2. **Extend: The Optional Twist**
   - Not every shopper wants the same experience. Some prefer gift wrapping for their orders, while others don’t. Alex created a use case called **Specify Gift Wrap**, which **extends** the main "Place Order" use case.
   - The main story could function perfectly without the extension, but for those who needed it, the extended sequence made the experience richer.

   *For example:*
   - Main Use Case: **Place Order**
   - Extending Use Case: **Specify Gift Wrap**

   This showed how Alex could add optional behaviors without overcomplicating the main flow.

3. **Generalization: The Family Tree**
   - Alex also discovered that not all orders were the same. Some customers wanted a one-time purchase, while others signed up for recurring subscriptions. Both these cases stemmed from the same parent story—**Place Order**.
   - Using **generalization**, Alex created child use cases like **Place Subscription Order** and **Place Single Order.** These inherited the steps of "Place Order" but added their unique details.

---

#### **Act 4: The Unexpected Turns (Scenarios)**

No story is complete without a few twists. Alex knew that the system wouldn’t always follow the ideal path. Each use case had to account for both the **happy path** (the perfect scenario) and **alternate flows** (unexpected challenges).

For "Place Order," Alex mapped:
- **Main Flow**: The shopper logs in, adds items, and successfully pays.
- **Alternative Flow 1**: The shopper’s payment is declined, and they’re prompted to retry.
- **Alternative Flow 2**: The selected item is out of stock, and the system suggests similar products.

This gave the system resilience, just like a well-prepared hero facing unforeseen obstacles.

---

#### **Act 5: Refining the Plot**

Alex polished the story further:
1. **Numbering the steps** for clarity.
2. **Writing failure conditions** as extensions, so every path was covered.
3. Keeping the language **clear and actor-focused**, avoiding technical jargon.

---

#### **Act 6: The Grand Blueprint**

By the end of the journey, Alex’s system had:
1. **Actors** who brought life to the story—shoppers, payment systems, and administrators.
2. **Use cases** that captured every interaction.
3. **Relationships** like:
   - **Include** for shared behaviors.
   - **Extend** for optional adventures.
   - **Generalization** for specialized scenarios.
4. **Scenarios** that prepared the system for both smooth and bumpy rides.

For example, Alex’s system for an **Online Recruitment System** featured:
- **Application Subsystem**: Use cases like "Register Applicant" and "Submit Application."
- **Selection Subsystem**: Use cases like "Rank Applications" and "Shortlist Candidates."
- **Administration Subsystem**: Use cases like "Add Reviewer" and "Assign Roles."

Each subsystem used **include** for common steps (e.g., "Log In"), **extend** for optional features (e.g., "Add Notes to Application"), and **generalization** for specialized roles (e.g., "Graduate Application" and "Undergraduate Application").

---

#### **Epilogue: The Golden Rules**
Alex reflected on the lessons learned:
1. Always write from the **actor’s perspective**.
2. Use **simple, active names** that describe the goal, not the process.
3. Keep the story clear, logical, and prepared for real-world complexities.

And so, with the use case model as the backbone, Alex built a system that didn’t just work—it thrived, delighting its users and proving that every great system begins with a great story.

---

### **Section 1: Basics of Use Cases**
1. **Question:** What is a use case, and why is it important in system design?  
   **Answer:** A use case is a goal-oriented sequence of interactions between actors and a system that yields a valuable result to the actor. It is important because it helps in understanding the system’s behavior, capturing and specifying requirements, and ensuring the system meets user needs.

2. **Question:** Who introduced the use case technique, and when?  
   **Answer:** The use case technique was introduced by Ivar Jacobson in 1992 as part of his Object-Oriented Software Engineering methodology.

3. **Question:** What is the difference between a primary actor and a secondary actor?  
   **Answer:** A primary actor interacts with the system to achieve a goal and derives direct benefit from it. A secondary actor supports the system or the primary actor but does not directly achieve a goal.

---

### **Section 2: Steps in Use Case Modeling**
4. **Question:** List the five steps in building a use case model.  
   **Answer:**  
   - Step 1: Identify and describe the actors.  
   - Step 2: Identify the use cases and write a brief description.  
   - Step 3: Identify the actor and use-case relationships.  
   - Step 4: Outline the individual use cases.  
   - Step 5: Refine the use cases.

5. **Question:** What are scenarios in the context of use cases? Provide an example.  
   **Answer:** A scenario is an instance of a use case representing a single path through it.  
   Example: For an ATM withdrawal use case:  
   - **Scenario 1:** Successful withdrawal.  
   - **Scenario 2:** Insufficient funds in the account.  
   - **Scenario 3:** ATM has insufficient cash.

---

### **Section 3: Relationships in Use Cases**
6. **Question:** What is an **Include** relationship in a use case? Provide an example.  
   **Answer:** An include relationship means that the behavior of one use case (the included use case) is reused by another (the base use case).  
   Example: The "Log In" use case is included in "Place Order" because logging in is required before placing an order.

7. **Question:** Explain the **Extend** relationship with an example.  
   **Answer:** An extend relationship allows one use case to add optional or conditional behavior to another.  
   Example: "Specify Gift Wrap" extends the "Place Order" use case, as gift wrapping is optional.

8. **Question:** What is the **Generalization** relationship in use cases? Provide an example.  
   **Answer:** Generalization is a parent-child relationship where the child use case inherits the parent’s attributes and behavior but may also add its own.  
   Example: "Place Subscription Order" generalizes the "Place Order" use case.

---

### **Section 4: Naming Use Cases**
9. **Question:** What are the guidelines for naming a use case?  
   **Answer:**  
   - Use verb-object format (e.g., "Buy Concert Ticket").  
   - Be specific and actor-focused.  
   - Avoid procedural names like CRUD (Create, Read, Update, Delete).  
   - Avoid system-centric names.

10. **Question:** Why is "Ticket Purchase" a poor name for a use case?  
    **Answer:** It is passive and lacks specificity about the actor’s intention. A better name would be "Purchase Concert Ticket."

---

### **Section 5: Practical Application**
11. **Question:** Describe the main success scenario and an alternative flow for the "Place Order" use case.  
    **Answer:**  
    - **Main Success Scenario:** The customer logs in, selects items, adds them to the cart, and completes the payment.  
    - **Alternative Flow:** The payment fails, and the system prompts the customer to retry or use another payment method.

12. **Question:** How does a system designer handle failure conditions in a use case?  
    **Answer:** Failure conditions are documented as extensions after the main success scenario, detailing what happens if a step fails.

---

### **Section 6: Examples and Subsystems**
13. **Question:** What are the key use cases in an Online Recruitment System’s Application Subsystem?  
    **Answer:**  
    - Register Applicant.  
    - Submit Application.  
    - Track Application.

14. **Question:** In the Online Recruitment System, what relationship exists between "Log In" and other subsystems?  
    **Answer:** "Log In" is included in all subsystems (Application, Selection, and Administration) because it is a common behavior.

15. **Question:** Which use case relationship best models optional behavior?  
    **Answer:** The **Extend** relationship is best suited for modeling optional behavior.

---

### **Section 7: Miscellaneous**
16. **Question:** What is the purpose of creating a system boundary in a use case model?  
    **Answer:** A system boundary defines the scope of the system and identifies what is inside (system functionality) and what is outside (external actors).

17. **Question:** Why is it important to refine use cases?  
    **Answer:** Refining use cases ensures clarity, completeness, and preparation for real-world scenarios. It involves detailing steps, addressing failure conditions, and improving readability.

18. **Question:** Differentiate between **Main Flow** and **Alternative Flow** in a use case.  
    **Answer:**  
    - **Main Flow:** The primary path where everything works as expected (e.g., successful order placement).  
    - **Alternative Flow:** Variations or failures that deviate from the main path (e.g., payment failure).

19. **Question:** How does **Include** differ from **Extend** in use cases?  
    **Answer:**  
    - **Include**: Adds mandatory, reusable behavior (e.g., "Log In" included in "Place Order").  
    - **Extend**: Adds optional or conditional behavior (e.g., "Specify Gift Wrap" extends "Place Order").

20. **Question:** What is the **Golden Rule** of use case names?  
    **Answer:** A use case name should indicate the value or goal achieved by the actor’s interaction with the system.


### **Conceptual Questions**

1. **What is a feasibility study?**
   - A feasibility study evaluates the practicality and viability of a project before commitment. It identifies potential benefits, technical challenges, and risks.

2. **What are the outcomes of a feasibility study?**
   - **Go ahead**: Proceed with the project.
   - **Do not go ahead**: Abandon the project.
   - **Think again**: Revise the plan.

3. **Why are feasibility studies challenging?**
   - **Uncertainty**: Benefits are hard to quantify; resource/timeline estimates are rough.
   - **Advocacy**: Stakeholders may overemphasize benefits and underplay risks.

4. **Why is scope important in feasibility studies?**
   - Scope defines project boundaries, avoiding misunderstandings about what is included/excluded.

5. **What questions do decision-makers need answered?**
   - **Client**: Who benefits?
   - **Scope**: What is included/excluded?
   - **Benefits**: What improvements will it bring?
   - **Technical Feasibility**: Can it be done?
   - **Resources**: What will it cost in terms of time, staff, and equipment?
   - **Alternatives**: What happens if we don’t proceed?

---

### **Practical Questions**

6. **What are common risks in feasibility studies?**
   - **Technical Risks**: Infrastructure compatibility, scalability issues.
   - **Organizational Risks**: Lack of expertise, resistance to workflow changes.
   - **External Risks**: Integration with external systems, legal/regulatory challenges.

7. **What makes a good feasibility report?**
   - **Concise and comprehensive**: Covers scope, benefits, risks, resources.
   - **Audience-focused**: Accessible for clients, technical teams, and managers.

8. **What should a preliminary plan include?**
   - Staffing and equipment needs.
   - Major milestones and deadlines.
   - External dependencies and deliverables.

9. **What are the benefits of a feasibility study?**
   - **Organizational**: Improved efficiency, reduced manual errors, faster response times.
   - **Technical**: Clear system design, informed decisions about tools and architecture.

---

### **Scenario-Based Questions**

10. **Steps to conduct a feasibility study for a payroll system?**
   - Define scope (e.g., payroll calculations, employee database).
   - Assess technical options (e.g., in-house or third-party development).
   - Identify risks (e.g., data migration).
   - Estimate resources (staff, timeline, cost).
   - Recommend alternatives or mitigations.

11. **How to handle technical risks identified during a feasibility study?**
   - Validate assumptions through prototypes.
   - Use phased implementation to test solutions incrementally.
   - Reassess timelines and adjust resources if needed.

---

### **Checklist Questions**

12. **Key checklist items for a feasibility study?**
   - Team availability and skills.
   - Timeline feasibility.
   - Equipment and software requirements.
   - Client involvement.
   - Startup needs (training, licenses, etc.).

13. **Key phases of a feasibility study?**
   - **Initiation**: Identify the problem and objectives.
   - **Analysis**: Assess scope, benefits, and risks.
   - **Feasibility Assessment**: Technical, organizational, and resource evaluation.
   - **Report Preparation**: Summarize findings and recommendations.
   - **Decision**: Go ahead, revise, or abandon.

---

### **Comparison Questions**

14. **Difference between organizational and technical feasibility?**
   - **Organizational Feasibility**: Focuses on readiness (e.g., skills, workflows).
   - **Technical Feasibility**: Focuses on system capability (e.g., design, scalability).

15. **Waterfall model vs. phased approach in risk management?**
   - **Waterfall Model**: Linear, assumes all requirements are known upfront, high risk if early stages fail.
   - **Phased Approach**: Incremental delivery, allows adjustments at each stage, reduces risk.

---

### **Critical Thinking Questions**

16. **Why can enthusiasm distort feasibility studies?**
   - Enthusiasm fosters advocacy but can lead to underestimating risks and overpromising benefits.

17. **How to improve the feasibility study process?**
   - Include diverse perspectives (technical, financial, client).
   - Use simulations or prototypes for validation.
   - Maintain transparency about risks and uncertainties.

---

