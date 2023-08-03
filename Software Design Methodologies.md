# **Software Design Methodologies**

## **Introduction**

Implementing a software design is a crucial phase in the software development process, where architects and engineers plan and define the structure of a system. Three popular design strategies are Structured Design, Function-Oriented Design, and Object-Oriented Design. Each approach offers unique principles and techniques to create effective and maintainable software solutions. 

### **What do we mean by coupling and cohesion when discussing structured design?**

**Coupling** is the extent to which two components depend on each other for successful execution; low coupling is good. For example, when you deliver a system and have to maintain it, if you change one module it is likely you have to change other modules.

**Cohesion** is the extent to which a component has a single purpose or function; high cohesion is good. For example, highly cohesive modules are much easier to reuse, they have a single purpose and you need to reuse them to accomplish that purpose. 


### **What is the difference between top-down and bottom-up design? Which best describes a function oriented design?**

**Top-Down Design:**
Top-Down Design starts with a broad view of the system and breaks it down into smaller, detailed components. It begins by identifying the main functionalities required to achieve the system's goals. These main functionalities are then divided into smaller sub-functionalities, and this process continues until the design reaches a level suitable for implementation. Essentially, top-down design involves dividing the system into manageable pieces based on its functional requirements.

Advantages:

1. Provides a clear understanding of the system's structure from the start.
2. Allows for a systematic and organized design approach.
3. Helps identify the essential functionalities early in the process.
4. Facilitates a modular and hierarchical design, making the system easier to maintain and extend.

**Bottom-Up Design:**
Bottom-Up Design begins by creating smaller, individual components (sub-components) that are later combined to form larger, more complex functionalities and the complete system. The focus is on developing and testing these smaller components independently before integrating them. In essence, bottom-up design involves combining smaller, tested components to build more significant and complex functionalities.

Advantages:

1. Promotes code reusability and modularity as smaller components can be reused in multiple contexts.
2. Allows developers to concentrate on detailed implementations of individual components.
3. Facilitates a more incremental and iterative development process.
4. Easier to test and debug smaller components before integrating them into the larger system.

**Function-Oriented Design and Top-Down Design:**
Function-Oriented Design works well with the Top-Down Design approach. In function-oriented design, the focus is on dividing the system into smaller functional units or procedures that perform specific tasks. These functions are then further organized into a hierarchical structure, starting from high-level functionalities to more detailed procedures. The design process follows a top-down approach, where the main functions are identified first and then decomposed into sub-functions until the system's design is sufficiently detailed for implementation.

In summary, Top-Down Design involves starting with a broad view of the system and breaking it down into smaller components, while Bottom-Up Design begins with smaller components and builds up to form the complete system. Function-Oriented Design best aligns with the Top-Down Design approach, as it revolves around dividing the system based on specific functions or procedures that perform distinct tasks.

### **In which design methodology would a class diagram be most useful?**

A class diagram is most useful in the Object-Oriented Design (OOD) methodology. In OOD, classes are used to model real-world entities or concepts as objects, encapsulating data and behaviors. The class diagram provides a graphical representation of the static structure of a system, illustrating classes, their attributes, methods, and relationships. It helps stakeholders understand the overall architecture, data structure, and interactions between components. Class diagrams play a significant role in the early stages of OOD, providing a blueprint for the implementation phase and guiding developers in writing code for classes and their interactions.

### **What are the four pillars of object oriented programming (OOP)? Give a single-sentence description of each.**

The four pillars of OOP are encapsulation, abstraction, inheritance and polymorphism. Below I describe them in more detail.

1. **Encapsulation:** Encapsulation is the bundling of data (attributes) and the methods (behaviors) that operate on that data within a single unit (class), hiding the internal details and exposing only the necessary interfaces to interact with the object.

2. **Abstraction:** Abstraction focuses on defining the essential characteristics and behaviors of an object, emphasizing "what" an object does rather than "how" it does it, allowing users to interact with the object without understanding its underlying complexities.

3. **Inheritance:** Inheritance enables a class (subclass) to inherit properties and behaviors from another class (superclass), promoting code reuse and creating a hierarchical relationship among classes.

4. **Polymorphism:** Polymorphism allows objects of different classes to be treated interchangeably through a common interface, enabling flexibility and dynamic behavior, where a single method can have different implementations depending on the object type it operates on.

### **What is the strategy pattern? How would its implementation differ between a functional and object oriented system?**

The Strategy Pattern is a behavioral design pattern that allows clients to choose from a family of algorithms or strategies interchangeably without modifying their code. It promotes flexibility by encapsulating each algorithm in a separate class, and clients can switch between these algorithms at runtime.

### **Imagine your is creating a new online payment system. In order to gain maximum market share it can't be tied to a particular sector - it needs to work just as well when ordering a takeaway as when buying a new coat. Which design methodology would you suggest following? Give some justification for your decision.**

For creating a new online payment system that needs to be versatile across different sectors, following the **Object-Oriented Design (OOD)** methodology may offer the best solution.

**Justification:**

1. Modularity and Reusability: OOD's modularity allows breaking down the system into smaller, self-contained classes for easy maintenance and code reusability.

2. Encapsulation and Abstraction: Encapsulation hides internal details, while abstraction provides a consistent interface for diverse payment methods.

3. Polymorphism: Polymorphism enables handling various payment types uniformly through common interfaces.

4. Inheritance: Inheritance allows sharing common functionalities while customizing features for specific sectors.

5. Flexibility and Future Expansion: OOD provides adaptability for integrating new payment methods and technologies.

6. Maintainability and Scalability: OOD promotes organized code, ensuring easy maintenance and scalability.

By following OOD, the payment system can achieve versatility, adaptability, and scalability across sectors while facilitating future enhancements.
