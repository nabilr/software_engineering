Here’s a well-organized, textbook-style explanation without slide numbers:

---

### Introduction to Use Cases
A **use case** is a structured interaction between an external actor and a system, aimed at achieving a specific goal. This concept was first introduced by Ivar Jacobson in 1992 and has since become a core part of object-oriented methodologies, including the Unified Software Development Process and the Unified Modeling Language (UML). Use cases capture **sequences of actions** that yield valuable outcomes for the actor involved. By emphasizing **external perspectives**, use cases focus on what the system does rather than how it functions internally. 

---

### Building a Use-Case Model – Step-by-Step
Creating a **use-case model** is a systematic process that involves the following steps:
1. **Identify and Describe the Actors** – Determine all parties that will interact with the system.
2. **Identify Use Cases and Provide Brief Descriptions** – Specify the interactions the actors will have with the system.
3. **Identify Actor and Use-Case Relationships** – Understand how each actor is related to each use case.
4. **Outline the Individual Use Cases** – For each use case, provide a detailed step-by-step narrative.
5. **Refine the Use Cases** – Make necessary adjustments to clarify and detail each use case.

This structured approach ensures that all user interactions are documented, providing a clear understanding of system requirements.

---

### Actors
**Actors** are external entities that interact with the system. They can be human users, roles played by users, or even other systems. Actors are classified as:
- **Primary Actors**: Those who interact directly with the system to achieve their objectives and are typically the main users.
- **Secondary Actors**: Entities that the system needs assistance from but do not directly benefit from the system. They support the primary actors’ goals.

This distinction clarifies which actors directly drive the system’s purpose versus those who play a supportive role.

---

### Primary vs. Secondary Actors
**Primary actors** engage with the system to achieve their goals and receive a direct benefit from it. For example, in an online shopping system, a customer would be a primary actor. In contrast, **secondary actors** do not benefit directly but are essential for primary actors to complete their tasks. In the same online shopping system, a payment processor would be a secondary actor as it supports the transaction process.

In UML diagrams, primary actors are usually placed on the left side, while secondary actors are typically on the right.

---

### Use Cases and Actor Relationships
In a **use-case model**, the system is viewed as a “black box.” This model only reflects external interactions, without delving into internal workings. Use cases capture:
- **Who** (actor) initiates or participates in the interaction,
- **What** (interaction) the actor does with the system,
- **Why** (goal) the actor initiates the interaction.

By defining these interactions, the use-case model illustrates how actors achieve their goals through system functions.

---

### Scenarios
A **scenario** is an instance or specific path through a use case. Each use case can contain multiple scenarios, such as:
- **Main Flow** – The primary path that achieves the use case's goal.
- **Alternative Flows** – Variations in the interaction that still fulfill the goal.

For example, in an ATM withdrawal use case, there might be scenarios for:
1. **Successful Withdrawal**,
2. **Insufficient Funds**, and
3. **Machine Out of Cash**.

This captures different conditions under which the interaction might proceed or fail.

---

### Golden Rule of Use-Case Naming
When naming a use case, ensure it reflects the **value or goal** achieved through the interaction. Questions to guide the naming include:
- Why is the actor interacting with the system?
- What goal is the actor aiming to achieve?
- What valuable outcome results from this interaction?

Use case names typically follow a **verb-object** format, such as “Buy Concert Ticket,” reflecting a process that yields a specific outcome for the actor.

---

### Naming Conventions
Use case names should:
- Be **complete** processes from the end user’s perspective.
- Use **active voice** to show direct actions.
- Be **specific** enough to convey what is happening.
- Reflect the **actor’s perspective**, not the system's internal workings.

For instance, “Purchase Concert Ticket” is better than “Ticket Order,” which sounds procedural and does not capture the end goal.

---

### CRUD Naming Issues
Avoid names based on CRUD (Create, Retrieve, Update, Delete) processes, as they do not describe actor intentions and are too procedural. For example, instead of “Create Account,” use “Register New User” to clarify the actor’s goal and the value they receive.

---

### Singular or Plural Naming
Choose between singular or plural use case names based on the context. For example:
- **“Buy Item”** at a vending machine (where only one item is bought),
- **“Buy Items”** in a supermarket context (where multiple items are bought).

The form should reflect the typical usage pattern of the system.

---

### Association Relationship
In UML, an **association** is a communication path between an actor and a use case. It is visually represented as a solid line and typically reads from left to right. This association shows which use cases each actor participates in and how they interact with the system.

---

### Use Case Structure
UML defines three relationships to structure use cases:
- **Include**: Integrates common functionality used by multiple use cases.
- **Extend**: Adds optional or conditional functionality to a use case.
- **Generalization**: Shows that one use case inherits characteristics from another.

These relationships help organize use cases and avoid redundancy.

---

### Include Relationship
The **include** relationship is similar to a subroutine call, where one use case calls upon another. For example, a “Place Order” use case may include “Log In” since the login process is necessary for multiple use cases, allowing reuse without duplication.

---

### Extends Relationship
An **extend** relationship specifies that one use case adds to the behavior of another but is not required for the base case. For example, “Specify Shipping Instructions” extends “Place Order” and only comes into play if the user chooses to add specific instructions.

---

### Include vs. Extends
- **Include** relationships are akin to a procedural call, where a common behavior is reused.
- **Extends** relationships add optional behaviors or enhance the base case conditionally.

Choosing the correct relationship allows for a more flexible and reusable use-case model.

---

### Generalization Relationship
A **generalization** relationship allows one use case to inherit properties from another. This is useful when a child use case needs to extend the parent’s behavior while still adhering to the parent’s general framework.

---

### Fire Alarm System Example
Use cases can be adapted to various systems, such as a fire alarm system, which involves actions like **activating alarms** and **notifying responders**. This shows how use cases apply across different domains and illustrate system behaviors.

---

### Building the Use Case Models
The process starts by defining a **system diagram** to outline system boundaries and actors, followed by **finding use cases** that specify how actors will interact. This forms the basis for the use-case model, which will eventually incorporate relationships and extensions.

---

### UGRU Online Recruitment System Example
An example of an online recruitment system with various actors (applicant, administrator, director) and subsystems (application, selection, and administration). This breakdown demonstrates how use cases apply to comprehensive systems.

---

### Subsystems
1. **Application Subsystem** - Focuses on actions such as **Registering** and **Tracking Applications**.
2. **Selection Subsystem** - Deals with **Ranking** and **Shortlisting Applications** by reviewers.
3. **Administration Subsystem** - Involves adding roles like **Admin** and **Director** and managing the application process.
4. **Editing Subsystem** - Allows for editing actions by the administrator.
5. **Viewing Subsystem** - For viewing users, applications, and statistics by administrative roles.

By detailing these subsystems, the document shows the breadth of interactions within a complex system, each facilitated by use cases that address specific actor needs.

--- 

This structure follows a traditional textbook format, thoroughly explaining each concept with relevant details and examples.
