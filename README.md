# Architecture Decisions
### Architecture decisions define the rules for `how a system should be constructed`.

Architecture decisions form `the constraints of the system` and direct the development teams on
`what is and what isn’t allowed`.

### 📏 วิธีการต่าง ๆ ในการสร้างระบบที่ผ่านการตัดสินใจ และสามารถบอกได้ว่าอะไรทำได้หรืออะไรทำไม่ได้

### Should use tools to help verify if someone breaks rules

### 🔍 ควรเครื่องมือตรวจสอบการทำงานว่าเป็นไปตามข้อกำหนด

---

# Design Principles
### Design principles are `guidelines for constructing systems`.

### เป็นหลักการหรือข้อแนะนำสำหรับการวางโครงสร้างระบบ

An exception to a particular `architecture decision is analyzed` by the ARB (or chief architect if no ARB exists) and is either approved or denied `based on justifications and trade-offs`.

### `Variance` can be defined to break the rule sometime

### 🚨 ถ้าวิเคราะห์แล้วพบว่ามีจุดที่ทำให้ต้องไม่ปฏิบัติตามข้อกำหนด (Variance) ก็ต้องมองหาสิ่งอื่นที่เหมาะสม (Design Principles)

---

# Expectations of an Architect
### roles and responsibilities of architects
The first key to effectiveness and success in the software architect role depends on understanding and practicing each of these expectations.

- ### Make Architecture Decisions
  An architect should `guide rather than specify technology choices` or might need to make specific technology decisions in order to preserve a particular architectural characteristic.
  ### 🤔 ตัดสินใจเกี่ยวกับเทคโนโลยีที่ทีมจะใช้ในการพัฒนาซอฟต์แวร์

- ### Continually Analyze the Architecture
  An architect is expected to continually analyze the architecture and current technology environment and `then recommend solutions for improvement`.

  An architect must holistically analyze changes in technology and problem domains to `determine the soundness of the architecture`. 
  ### 🔍 คอยวิเคราะห์สถาปัตยกรรมเพื่อดูความมั่นคงของระบบ และแนะนำวิธีแก้ไข

- ### Keep Current with Latest Trends
  The decisions an architect makes tend to be long-lasting and difficult to change. Understanding and following key trends helps the architect `prepare for the future and make the correct decision`.
  ### 📈 เสพข่าวสำคัญอยู่เสมอ เพื่อการตัดสินใจที่แม่นยำ

- ### Ensure Compliance with Decisions
  Continually verifying that development teams are following the architecture decisions and design principles defined, documented, and communicated by the architect.

  `By not ensuring compliance with architecture decisions`, the architecture `will not meet the required architectural characteristics` (“-ilities”), and the application or system `will not work as expected`.
  ### ✅ ตรวจสอบว่าทีมทำตามที่สถาปนิกกำหนดอย่างสมํ่าเสมอ ซอฟต์แวร์จะได้ตอบโจทย์กับความต้องการของระบบ

- ### Diverse Exposure and Experience
  An architect must at least be familiar with a variety of technologies. Focusing on `technical breadth rather than technical depth`.
  ### 🗺️ มีความรู้และประสบการณ์ในหลายด้าน เช่น ข้อดี ข้อเสีย ของเทคโนโลยีต่าง ๆ แต่ไม่จำเป็นต้องรู้ลึกทุกเรื่อง

- ### Have Business Domain Knowledge
  `Without business domain knowledge`, it is difficult to understand the business problem, goals, and requirements, making it `difficult to design an effective architecture to meet the requirements of the business`.

  `Without this knowledge`, an architect cannot communicate with stakeholders and business users and will `quickly lose credibility`. 

  Using the domain knowledge and `language that these stakeholders know and understand`.
  ### 👨‍💼 มีความรู้ด้านธุรกิจ เพื่อการออกแบบที่มีประสิทธิภาพ และสามารถสื่อสารกับผู้มีส่วนได้ส่วนเสียโดยใช้ภาษาที่เข้าใจได้ตรงกัน

- ### Possess Interpersonal Skills
  Including teamwork, facilitation, and leadership. `Leading the development teams through the implementation of the architecture`.
  ### 🫂 สามารถนำทีมให้ปฏิบัติตามแผนทางสถาปัตยกรรมได้ สื่อสารให้ทีมเข้าใจถึงการตัดสินใจและแนวทางต่าง ๆ ได้

- ### Understand and Navigate Politics
  The main point is that `almost every decision an architect makes will be challenged` by developers who feel their approach is better or due to `increased costs` or `increased effort (time)` involved.

  The architect must navigate the politics of the company and `apply basic negotiation skills to get most decisions approved`.
  ### 🤌 ควรมีทักษะการเจรจาเพื่อทำให้การตัดสินใจ (ที่มักจะโดนขัดจากปัญหาต่าง ๆ) ถูกอนุมัติหรือเห็นตรงกัน

---

# Architectural Thinking
### It is seeing things with an architectural eye, or an architectural point of view. 

- ### Architecture Versus Design
  The architect and developer must be on the same virtual team to make this work.

![Architecture Versus Design](images/arch-vs-design.png)

  An architect is responsible for things like `analyzing business requirements to extract and define the architectural characteristics` (“-ilities”), `selecting which architecture patterns and styles would fit the problem domain`, and `creating components` (the building blocks of the system). _The artifacts created from these activities are then handed off to the development team_, which is responsible for `creating class diagrams for each component`, `creating user interface screens`, and `developing and testing source code`.

  ### 👬 สถาปนิกควรสื่อสารกับนักพัฒนาให้บ่อย เพื่อให้เห็นภาพการทำงานที่ตรงกัน

- ### Technical Breadth
  A software architect must `have a significant amount of technical breadth` to think like an architect and see things with an architecture point of view.

![Technical Breadth](images/knowledge-pyramid.png)

  Architects also need to balance their knowledge. They shouldn't spread themselves too thin trying to learn everything, but they also shouldn't focus too narrowly on just one thing. Finding the right balance between `knowing a lot about a few things (depth)` and `knowing a little about many things (breadth)` is important for their career growth.

  ### ⚖️ สถาปนิกควรรู้ให้กว้างในหลาย ๆ เรื่อง และรู้ลึกเพียงบางเรื่องก็พอ

- ### Analyzing Trade-Offs
  Thinking like an architect is all about seeing trade-offs in every solution, technical or otherwise, and analyzing those trade-offs to determine what is the best solution. `There are no right or wrong answers` in architecture—only trade-offs.

![Analyzing Trade-Offs](images/topic-pros-cons.png)

  Thinking like an architect is analyzing these trade-offs, then asking “`which is more important`: extensibility or security?” The decision between different solutions will always `depend on the business drivers, environment, and a host of other factors`.

  ### 📊 พยายามวิเคราะห์ข้อดีข้อเสียของแต่ละวิธีการ โดยมองจากตัวแปรต่าง ๆ และสร้างทางที่ดีที่สุด

- ### Understanding Business Drivers
  This is a challenging task that requires the architect to have `some level of business domain knowledge` and `healthy collaborative relationships with key business stakeholders`.

  ### 👨‍💼 เข้าใจว่าอะไรที่ขับเคลื่อนธุรกิจให้ไปต่อได้

- ### Balancing Architecture and Hands-On Coding
  - `Avoid the Bottleneck Trap`:
    
    delegate writing critical code to developers, and focus on software architecture.

    - ### โฟกัสงานหลัก
    
  - `Proof-of-Concepts (POCs)`:
    
    try out different solutions to see which one is the best

    - ### ทดลองหาวิธีการใหม่ ๆ
    
  - `Tackling Technical Debt`:
    
    fix small issues (technical debt) in the codebase, keeping things running smoothly.

    - ### ไม่มักง่ายในการเขียนโค้ด (คิดถึงปัญหาในอนาคตเสมอ)
    
  - `Bug Fixes`:
    
    fixing bugs makes understanding where the weaknesses are in the codebase and how to improve them.

    - ### แก้บัค หาข้อด้อยในโค้ด (เขียนให้ดูเป็นตัวอย่าง ทำโค้ดรีวิว)
    
  - `Automation`:
    
    creating command-line tools and analyzers for day-to-day tasks, or using fitness functions.

    - ### ใช้เครื่องมือช่วยเหลือ

---

# Modularity
### Each of a set of `standardized parts or independent units` that can be used to construct a more complex structure.

## Measuring Modularity

- ### Cohesion
  > It is a measure of how related the parts are to one another.

  ### A range of cohesion measures from best to worst (some examples):

  - ### Functional cohesion

    Every part of the module is related to the other, and the module contains everything essential to function.

    ### ทุกฟังก์ชันมีความเกี่ยวข้องและทำงานไปในทางเดียวกัน
  
  - ### Sequential Cohesion

    Two modules interact, where one outputs data that becomes the input for the other.

    ### มีโมดูลหนึ่งที่ส่งผลลัพธ์ให้กับอีกโมดูลไปทำงานต่อ

  - ### Communicational Cohesion

    Two modules form a communication chain, where each operates on information and/or contributes to some output.

    ### ทั้งสองโมดูลทำงานต่อกัน (ประสานงานร่วมกัน)
  
    ### LCOM (Lack of Cohesion in Methods)

      the sum of the sets of `methods not shared via sharing fields`

      ### จำนวนของกลุ่มเมธอดที่ไม่ได้เรียกใช้แอตทริบิวต์ตัวเดียวกัน (dissimilar - similar)
      ### ยิ่งความสัมพันธ์มาก ค่า LCOM ยิ่งตํ่า นับว่าดี

- ### Coupling
  - ### Afferent coupling:
    number of `incoming connections` to a code artifact (component, class, function, etc.)
  
  - ### Efferent coupling:
    number of `outgoing connections` to other code artifacts

  #### `จำไว้ว่า ควรถูกเรียกใช้ > ใช้ส่วนอื่น`

  - ### Abstractness (วัดความชัดเจน)
    the ratio of abstract to concrete artifacts

    #### too many abstractions, makes it difficult to understand how things wire together

    #### ยิ่งไม่ชัดเจน ยิ่งยากจะเข้าใจความสัมพันธ์

  - ### Instability (วัดความมั่นคง)
    the ratio of outgoing to all coupling

    #### high volatility breaks more easily

    #### พึ่งพามากเกินไป ทำให้พังง่ายกว่าเดิม

  - ### Distance from the Main Sequence
    relationship between abstractedness and instability

    #### หาตรงกลางระหว่างความชัดเจนและความมั่นคง

- ### Connascence
  > Two components are connascent if a change in one would require the other to be modified in order to maintain the overall correctness of the system.

  ### ความยึดติดกันระหว่าง component (ฉันเปลี่ยน เธอต้องเปลี่ยน)
  - ### Static Connascence

    - **Connascence of Name (CoN)**: เปลี่ยนชื่อ

    - **Connascence of Type (CoT)**: เปลี่ยนเดต้าไทป์

    - **Connascence of Meaning/Convention (CoM/C)**: เปลี่ยนกฎที่คนส่วนใหญ่ยึดตาม

    - **Connascence of Position (CoP)**: เปลี่ยนลำดับพารามิเตอร์

    - **Connascence of Algorithm (CoA)**: เปลี่ยนขั้นตอนวิธีการทำงานของโค้ด

  - ### Dynamic Connascence - runtime coupling

    - **Connascence of Execution (CoE)**: เปลี่ยนลำดับคำสั่ง

    - **Connascence of Timing (CoT)**: เปลี่ยนเวลาในการทำงาน เช่น race condition, asynchronus

    - **Connascence of Values (CoV)**:
    เปลี่ยนค่าไม่ครบทุกส่วนที่ระบบต้องการ

    - **Connascence of Identity (CoI)**:
    เปลี่ยนการอ้างถึงออบเจ็กต์ไม่ครบทุกส่วนที่ระบบต้องการ

- ### Connascence Properties
  - **Strength**: ทำให้ง่ายต่อการ refactor code
  - **Locality**: ระยะห่างของ connascence ที่เกิดขึ้นระหว่าง component มีผลต่อความเสียหายของระบบ
  - **Degree**: ยิ่งมี connascence ที่มากหรือสูง โอกาสเกิดความเสียหายก็เพิ่มตาม