### Assignment 2 Reflection
Running this project was challenging due to errors caused by syntax, logic, dependencies, or configuration issues. Despite debugging, testing, and consulting documentation and forums, I couldn't get it to run. AI was invaluable for breaking down problems and offering step-by-step guidance, while documentation and online communities provided deeper insights and practical examples. Tutorials and guides helped clarify foundational concepts.

When stuck, I learned the importance of persistence, taking breaks, and seeking clarification. These challenges taught me to use resources effectively and view failures as learning opportunities.

Acknowledgments: Thanks to Shasha, Siya, the open-source community, and online resources for their support and tools that enhanced my understanding.

### Assignment 5 Reflection
Putting the idea on paper was super exciting, but the implementation was super challenging. Having Math symbols on the system was a super challenging implementation. The choice of the backend language and the database a challenging; ultimately, JavaScript wins.

### Assignment 7 Reflection
I tried to make/export a Kanban board to an .md file, but it doesn't show as it is on the projects. Please refer to the one in the projects. I made projects accessible for reference, as they show exactly what I did. I learnt that system design and system development need extensive research on how user needs or conceptual ideas would be transformed into a real-life system. User requirements are huge when it comes to system design. One has to do extensive research, otherwise, the system may not serve what it was developed for.

###  Assignment 9: Reflection on Domain Modeling and Class Diagram Design

#### 1. Challenges Faced in Designing the Domain Model and Class Diagram

Designing the domain model and translating it into a class diagram for *Math Booster* presented several challenges, particularly in the areas of **abstraction**, **method definition**, and **relationship modeling**. One major challenge was determining the level of abstraction for each domain entity. For example, deciding whether `Learner` and `Educator` should be independent entities or inherit from a generic `User` class required careful thought. Initially, it seemed simpler to define them as separate classes with repeated fields such as email and password. However, this approach quickly led to redundancy and poor scalability. The decision to use inheritance improved cohesion and maintained a cleaner model, but required additional thought about shared versus specific behaviors.

Another challenge was defining **relationships and multiplicities**. For instance, the `Submission` entity is linked to both `Assessment` and `Learner`, and it also interacts with the `OTP` entity for secure verification. Capturing this triad relationship correctly, while ensuring the OTP logic remained encapsulated and did not complicate the Submission class excessively, required both structural and functional considerations. It was also difficult to balance complexity when modeling features like `Notifications` and `Reports`, which touch multiple actors and use cases. Keeping them generic and decoupled helped maintain flexibility.

Defining methods for each class was another sticking point. While CRUD operations are implicit, the functional methods are  needed to reflect real user interactions. For example, determining whether the method `submitAssessment()` should live on the `Learner` class or be an operation triggered via the `Assessment` class (based on action ownership) was a conceptual hurdle. Eventually, focusing on who initiates the action—typically the actor in the use case—helped guide method placement.

#### 2. Alignment with Previous Assignments

The class diagram aligns strongly with prior assignments, particularly the **use case specifications**, **functional requirements**, and **stakeholder concerns**. Each primary actor in the use cases—Learner, Educator, System Administrator, and Developer—has a corresponding domain class, and the methods within each class are modeled directly from the use case actions. For instance, `submitAssessment()` maps directly to the "Submit" use case, while `generateReport()` reflects the "Reports Generation" flow.

Furthermore, non-functional requirements like secure authentication and school-domain-based registration informed the inclusion of attributes like `passwordHash`, `email`, and `OTP`. Stakeholder feedback around automation, learner monitoring, and system performance shaped choices such as the inclusion of the `Notification` and `Report` entities.

The diagram also conceptually supports activity/state diagrams—for example, submission status changes ("Pending" → "Submitted" → "Marked") can be represented by the `status` attribute in `Submission` and managed by its methods.

#### 3. Trade-Offs Made

A major trade-off was **simplifying the inheritance structure**. Although the system supports various roles (Learner, Educator, Admin, Developer), the class diagram models only two user types via inheritance from `User`. A more complex role-based access control (RBAC) system could be implemented using interfaces or mixins, but this would introduce unnecessary complexity at the domain modeling stage.

Another trade-off was the **flattening of relationships** for clarity. For example, the `Assessment` class does not explicitly model classroom or subject groupings, which might exist in a full school system. This choice was made to keep the model focused on the core functionality: learning and assessment.

Additionally, rather than representing messaging and chat systems in full depth (e.g., threads, message history), a simple `Notification` class was used to acknowledge user communications. This simplification keeps the system focused and avoids unnecessary over-engineering.

#### 4. Lessons Learned

This project provided strong insights into the **principles of object-oriented design**, especially the importance of **encapsulation, abstraction, and responsibility-driven design**. By structuring responsibilities around actors and their behaviors (e.g., submitting, marking, reporting), the domain model remains intuitive and aligned with business logic.

The use of **inheritance** improved reusability but also highlighted the importance of clear class boundaries. Meanwhile, working through associations and multiplicities emphasized the need for precision, especially when modeling many-to-many or optional relationships.

Overall, this exercise demonstrated how domain modeling is not just a technical task but also a critical bridge between stakeholder needs, system behavior, and software architecture. It reinforced the importance of **iterative refinement**—starting simple and expanding based on validated requirements.

Lastly, the use of **Mermaid.js** for visual representation was a valuable lesson in maintaining **clarity and communication**. A well-documented diagram doesn’t just serve developers—it communicates design rationale to all stakeholders in the software development lifecycle.
