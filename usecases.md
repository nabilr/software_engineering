### Introduction to Use Cases
**Remember**: A use case captures the **interaction** between the user and the system, focusing on what the user wants to achieve without detailing how the system performs it.

- **Example**: For an **online shopping system**, a use case like **“Place Order”** involves selecting items, adding them to a cart, and completing a purchase. 
  - **UML Diagram**: In a UML use case diagram, the **Customer** would be represented by a stick figure labeled “Customer,” connected by a line to an oval labeled “Place Order,” indicating that the customer interacts with this functionality.

---

### Building a Use-Case Model – Step-by-Step
**Remember**: Building a use-case model follows a process:
1. **Identify Actors** – Who will use the system?
2. **Identify Use Cases** – What actions will they take?
3. **Define Relationships** – How do actors and use cases connect?
4. **Outline Use Cases** – What are the step-by-step actions?
5. **Refine Details** – What could go wrong or vary?

- **Example**: In a **hotel booking system**:
   - **Identify Actors**: Customer and Receptionist.
   - **Identify Use Cases**: Actions might include **“Book Room”** and **“Cancel Reservation.”**
   - **Define Relationships**: The Customer is the primary actor for “Book Room,” while the Receptionist might assist in “Cancel Reservation.”
   - **Outline Use Cases**: “Book Room” might involve selecting a room, entering payment details, and confirming the reservation.
   - **Refine Details**: Add scenarios like what happens if no rooms are available.

  - **UML Diagram**: A UML diagram would show two stick figures labeled **Customer** and **Receptionist**, each connected to oval shapes labeled “Book Room” and “Cancel Reservation.” This visualizes the actions each actor takes with the system.

---

### Actors
**Remember**: **Actors** are the people or systems that **interact** with the system. They can be **primary** (directly benefiting from the system) or **secondary** (supporting the primary actors).

- **Example**: In a **university registration system**:
   - **Primary Actor**: **Student**, who registers for courses.
   - **Secondary Actor**: **Registrar**, who verifies and processes registrations.
   
  - **UML Diagram**: In the UML use case diagram, both **Student** and **Registrar** would appear as stick figures. The **Student** would connect to “Register for Course,” while **Registrar** might connect to “Verify Registration,” showing their respective interactions.

---

### Primary vs. Secondary Actors
**Remember**: A **primary actor** is the main user seeking a specific result, while a **secondary actor** helps them achieve it but does not directly benefit.

- **Example**: In a **food delivery app**:
   - **Primary Actor**: The **Customer**, who orders food.
   - **Secondary Actor**: The **Delivery Driver**, who provides the delivery service.
   
  - **UML Diagram**: The **Customer** stick figure would be connected to the “Order Food” use case oval, and the **Delivery Driver** would connect to an oval labeled “Deliver Food,” indicating how they each interact with different parts of the system.

---

### Use Cases and Actor Relationships
**Remember**: A **use-case model** describes who interacts with the system, what they do, and why. It captures the **goal** the actor wants to achieve.

- **Example**: For a **movie ticket booking system**:
   - **Actor**: The **User**, who buys a ticket.
   - **Interaction**: The user selects a movie, chooses seats, and completes payment.
   - **Goal**: Reserve seats for a movie.
   
  - **UML Diagram**: The **User** stick figure would connect to multiple ovals: “Select Movie,” “Choose Seats,” and “Make Payment.” Arrows would represent the flow of interactions in sequence, showing the steps involved in achieving the goal.

---

### Scenarios
**Remember**: Each **use case** can have different **scenarios** or paths. There’s a main path (the goal) but also alternatives for what happens under varying conditions.

- **Example**: In an **ATM withdrawal system**:
   - **Main Scenario**: The customer successfully withdraws cash.
   - **Alternative Scenarios**: The system could decline if there are insufficient funds or if the ATM is out of cash.
   
  - **UML Diagram**: The **Customer** stick figure would connect to “Withdraw Cash.” Inside “Withdraw Cash,” you might see smaller ovals or notes showing alternate flows, like “Error: Insufficient Funds” and “Error: ATM Out of Cash.”

---

### Golden Rule of Use-Case Naming
**Remember**: Name a use case to clearly show the **goal or value** achieved by the actor. Use a **verb-object** format like “Track Order” to describe what the actor is doing.

- **Example**: In an **e-commerce platform**:
   - **Good Name**: **“Track Order”** – Clearly reflects what the user wants to do.
   - **Poor Name**: **“Order Tracking”** – Sounds procedural and less intuitive for the user.
   
  - **UML Diagram**: The **Customer** stick figure would connect to “Track Order” in the UML diagram, making it clear that this is an action they directly perform.

---

### Naming Conventions
**Remember**: Use case names should be **active**, **specific**, and from the **actor’s perspective**. This makes it clear what the actor is doing in the system.

- **Example**: In a **content management system**:
   - **Preferred Name**: **“Publish Article”** – Active and descriptive of the user’s action.
   - **Less Effective Name**: **“Article Publishing”** – Passive and doesn’t emphasize the actor’s role.
   
  - **UML Diagram**: The actor (e.g., **Editor** stick figure) would connect to “Publish Article,” showing a clear action in the diagram.

---

### CRUD Naming Issues
**Remember**: Avoid **CRUD terms** (Create, Retrieve, Update, Delete) alone, as they don’t indicate the **purpose** or goal. Instead, use names that show **intent**.

- **Example**: In a **customer management system**:
   - Instead of **“Create Contact,”** use **“Add New Contact”** to clarify the actor’s goal.
   
  - **UML Diagram**: The actor (e.g., **Admin** stick figure) connects to “Add New Contact” rather than “Create Contact,” making the action clear and purpose-driven in the use case model.

---

### Singular or Plural Naming
**Remember**: Choose **singular or plural** based on how users typically interact with the system. This makes the name more intuitive.

- **Example**: In a **retail checkout system**:
   - Use **“Purchase Item”** for single-item purchases, like a vending machine.
   - Use **“Purchase Items”** for multi-item purchases, like a supermarket.
   
  - **UML Diagram**: The **Customer** would be connected to either “Purchase Item” or “Purchase Items,” depending on the typical usage. This helps the actor understand the action more easily.

---

### Association Relationship
**Remember**: An **association** shows the **communication** between an actor and a use case, often represented by a line in UML diagrams.

- **Example**: In a **library management system**, the **association** between the “Student” actor and “Borrow Book” use case is a line connecting them, showing the interaction path.
  
  - **UML Diagram**: The **Student** stick figure would connect to “Borrow Book” with a line, indicating the student’s participation in the system.

---

### Use Case Structure
**Remember**: Use cases can have three main relationships:
1. **Include**: For reusing common steps.
2. **Extend**: For adding optional or conditional steps.
3. **Generalization**: For cases where one use case inherits from another.

- **Example**: In an **e-commerce website**:
   - **Include**: “Log In” might be included in use cases like “Place Order” and “View Order History.”
   - **Extend**: “Choose Gift Wrap” might extend “Purchase Item” as an optional step.
   - **Generalization**: A general “Purchase” use case could lead to “Purchase Physical Item” or “Purchase Digital Item.”
   
  - **UML Diagram**: Each relationship would be shown with different UML notations: dashed arrows for “Include” and “Extend,” and a line with a hollow arrowhead for “Generalization.”

---

### Include Relationship
**Remember**: **Include** means the use case **reuses common steps** or sub-actions. It’s like a subroutine in a program.

- **Example**: In a **food delivery app**, **“Order Food”** might **include** “Log In,” since logging in is required for other actions like ordering or updating details.
  
  - **UML Diagram**: “Order Food” would have a dashed arrow pointing to “Log In,” indicating that “Log In” is a reusable subroutine within “Order Food.”

---

### Extends Relationship
**Remember**: **Extend** adds **optional** or **conditional** steps to a base use case. It’s used for actions that only occur under certain conditions.



- **Example**: In an **online bookstore**, **“Buy Book”** could **extend** to “Gift Wrap Option,” which only happens if the user selects it.
  
  - **UML Diagram**: “Gift Wrap Option” would have a dashed arrow labeled <<extend>> pointing back to “Buy Book,” indicating that this is an optional behavior linked to the main purchase.

---

### Include vs. Extends
**Remember**: 
- **Include**: Always needed and reusable, like a common subroutine.
- **Extend**: Adds behavior that is optional or conditional, activated only in specific cases.

- **Example**: In a **travel booking system**:
   - **Include**: “Book Flight” might include “Enter Payment Details” because payment is always required.
   - **Extend**: “Choose Seat” might extend “Book Flight” if seat selection is optional.
   
  - **UML Diagram**: “Book Flight” would include “Enter Payment Details” with a dashed arrow pointing to it. “Choose Seat” would extend “Book Flight” with a dashed arrow indicating optional behavior.

---

### Generalization Relationship
**Remember**: **Generalization** lets one use case **inherit steps** from another, like a parent-child relationship. It’s useful for shared core behaviors.

- **Example**: In a **restaurant reservation system**:
   - A general “Make Reservation” use case could have specialized versions like “Make Dine-In Reservation” or “Make Takeout Reservation.”
   
  - **UML Diagram**: “Make Dine-In Reservation” and “Make Takeout Reservation” would connect to “Make Reservation” using lines with hollow arrowheads, representing inheritance.

---

### Fire Alarm System Example
**Remember**: Use cases can apply to **different domains**. They capture various responses and actions required for different scenarios.

- **Example**: In a **fire alarm system**, a primary use case might be **“Trigger Alarm,”** connected to other use cases like **“Notify Fire Department”** and **“Evacuate Building.”**
  
  - **UML Diagram**: **Trigger Alarm** would connect to **Notify Fire Department** and **Evacuate Building** with association lines, representing the actions triggered by an alarm activation.

---

### Building the Use Case Models
**Remember**: Begin by **defining the system boundaries and actors**, then identify the interactions to form the foundation of the use-case model.

- **Example**: In a **hospital management system**:
   - **Actors**: Doctors, Patients, and Nurses.
   - **Use Cases**: “Schedule Appointment” and “Access Patient Records.”
   - **Relationships**: Show which actor is responsible for which use case.
   
  - **UML Diagram**: The diagram would include stick figures for **Doctors, Patients,** and **Nurses** connected to the respective use cases they interact with, such as “Schedule Appointment.”

---

### UGRU Online Recruitment System Example
**Remember**: Use cases help illustrate **complex systems** with different actors and stages. They support comprehensive processes by organizing interactions and detailing relationships.

- **Example**: In a **recruitment system**, actors like **Applicant, Administrator,** and **Director** interact with use cases like **“Submit Application,”** **“Review Application,”** and **“Select Candidate.”**
  
  - **UML Diagram**: The diagram would feature stick figures for **Applicant, Administrator,** and **Director** with association lines to various ovals like “Submit Application” or “Select Candidate,” showing their specific interactions.

---

### Subsystems
**Remember**: Complex systems often include subsystems grouping related interactions.

- **Example**: In a **university application system**, the **Application Subsystem** might involve “Submit Application” and “Track Status.”
  
  - **UML Diagram**: A larger oval labeled **Application Subsystem** would contain smaller ovals for each individual use case within it. The **Student** actor would connect to the **Application Subsystem** with lines to the various contained use cases like “Submit Application.”

---

These explanations and UML diagram descriptions offer a practical approach to understanding each concept and how it visually represents the system's interactions.
