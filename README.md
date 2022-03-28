# Applied System Software

[Prof. Aleksejs Jurenoks](mailto:aleksejs.jurenoks@rtu.lv)  

Your total score depends on 3 factors:
-  All works completed on time, observing ORTUS deadlines - 30%
-  Two tests that will be evaluated with a mark - 30%
-  Final exam in the Online environment - 40%.

relevant course: https://github.com/gabboraron/halado_szoftvertechnologiak

## What is application and what is Software
requireeóments are constantly changing

Lifecycle
- conception
- childhood
- adulthood
- retirement


which activites should we select forthe software project? what are the dependencies between them? how should we schedule the activites?

funcional modeling of software lifecycl
- scenarios
- use case model

structural modeling of software lifecycle
- object identification
- class diagrams

dynamic modeling of software

questions:
- What is the problem?
- what is the solution?
- what are the best mechanisms to implement? - languages/API
- how is the solution constructed? - 
- is the roblem solved?
- can costumeruse the slution?
- how dowe deal with changes?

soft dev activities:
- requirements
- system design
- detailed design
- program implenetation
- testing
- delivery
- maintenence

waterfall model to vmodel

## concept proposal of a *New text editor software system*
[concept_proposal.doc](https://github.com/gabboraron/Applied_System_Software/blob/main/concept_proposal.doc)

## requirement analysis
bridging gap between system requirements enineering ad  software design

- sstem information
- function
- behavior

model -> data

**objectives:**
- identify customer's needs
- evaluate system for feasibility
- perform economic and technical analysis
- allocate functions to system elements
- estabilish schedule and constraints
- create system definitions

**software requirements analysis phases:**
1. **problem recognition:** what do you want to solve
2. **evaluation and synthesis**: how it is implemented, what kind of models do we used for
3. **modeling:** how and what system can handle it? 
4. **specification**
5. **review**

management questions:
- how much effort put towards analysis?
- who does the analysis?
- whhy is it so difficult?
- who pays for it?

**feasibility study:**
- economic feasiblity: cost benefit analysis
- technical: hardware/software/people
- legal:what acan we do, GDPR, etc
- alterantives: there is always more than one way to do it

**system specification:**
- functional data tdescription
- subsystem description
- system modeling and simulation results
- products
- appendices

**requirements:** 
- features of system or function used to fulifill system purpose
- focus on user's needs and not on solution

**types ofrequirements:**
- **functional**
  - input/output
  - processing
  - error handling
- **non functional requirements**
  - physical enviroment
  - interfaces
  - user/human factors
  
**requirement  definition:**
- general purpos of document
- system background and objectives
- description of approach
- detailed characersitics

**software requirements elicitation**
- customer meetings are most commonly usued 
- context free 

***FAST**
- fascilitated application specification technque
- meeting between customer and dev at neutral site
- gals:
  - identify probelem
  - propose elements of solution
  - negotiae different appproaches
  - specify preliminary set of requirements

**QFD**
- quality function development
- customer's needs impply technical requirements:
  - normal requirements
  - expected requirements
  - exciting requirements

**use cases**
- scenraios that describe how the product will be used
- written narratives that describe the role of an actor
- use cass designed from the actor's point of view
- not all actors can be identified during the fst iteration of requirements 
- identify the firs actors feore creating the first use-cases

**profiels:**
- full control: administrator
- read/write/modify all manager
- read/write/modify own inspector
- read only

**information domain**
- encompasses all data objects that contain numbers text images audio or video
- content/data model
- information flow
- information structure

**modelling**
- data model
- functional model
- behavioral model

**specificrepresentation**
- representation format and content
- information contained within the specification should be nested
- diagrams and other noational forms should be restricted in number and consistent use

**specfication**
- conducted by custemer and software developer
- once approved the specs becomes a contract for software development
- the specification is difficult to test in a meaningful way
- assessing the impact of specification changes is hard to do

## User Interface Analysis and Design
*ex: how MS Word communicate with MS Excel*

text based interface simplifes the interaction; easyer to teach

### user interface development - spiral process
- Interface analysis (user, task, and environment analysis)
  - Focuses on the profile of the users 
  - Concentrates on users, tasks
  - Studies different models of system function
- Interface design: set of interface objects and actions
- Interface construction begins with a prototype that enables usage scenarios
- Interface validation

based on user:
- Define interaction modes
- The user shall be able to perform the same action via keyboard, mouse, voice recognition
- Allow user interaction to be interruptible and "undo"able
- allow the interaction to be customized
- Hide technical internals from the casual user
- Design for direct interaction with objects that appear on the screen

Reduce the User's Memory:
- Reduce demand on short-term memory
- Establish meaningful defaults
- Define shortcuts that are intuitive
- The visual layout of the interface should be based on a real world metaphor
- Disclose information in a progressive fashion

Make the Interface Consistent:
- The interface should present and acquire information in a consistent fashion
- Allow the user to put the current task into a meaningful context
  - able to communicate with the software; 
- Maintain consistency across a family of applications *MS Office - Word - Excel, PowerPoint, etc in one line*
- If past interactive models have created user expectations, do not make changes unless there is a compelling reason to do so!

Models:
- User profile model – Established by a human or software engineer
- Design model – Created by a software engineer
- Implementation model – Created by the software implementers
- User's mental model – Developed by the user when interacting with the application

Analysis: if the interface fulfill the enviroments
- The users who will interact with the system through the interface
- The tasks that end users must perform to do their work
- The content that is presented as part of the interface
- The work environment in which these tasks will be conducted

user interface information can be obtained from
- User interviews with the end users
- Sales input from the sales people who interact with customers
- Marketing input based on a market analysis to understand how different population segments might use the software
- Support input from the support staff who are aware of what works and what doesn't

Work Environment: different UI on Win/Mac/ubuntu/android/ios

[10 Usability Heuristics for User Interface Design](https://www.nngroup.com/articles/ten-usability-heuristics/)

## Security
![increasing security threats](https://www.iacpcybercenter.org/wp-content/uploads/2015/04/deloitte-nascio-fig29.png)

http://www.ganssle.com/

Security vulnerabilites are to be cosdered bugs, the same way as a functional bug, and tracked in the same manner.

Factor some time into the project plan for security.
Consider security as added value in an application.

![software security tollgates in the sdlc](https://image.slideserve.com/396380/slide10-l.jpg)

### application security risk categorization
- more security for riskier applications
- ensures that you work the most critical issues first
- scales to houndreds or thousands off applications

tools and methods:
- security profiling tools gan gather facts  like size cpmplexity, security, mechanisms, dangerous calls
- questionnaire to gather risk informations: asset value, available functions, users, environment, threats
- risk based approach: evaluates likelihood and consequneces of successful attack

start the generic set  of security requirements
- include all sec mechanisms
- address all common vulnerabilities
- should address driving requirements

tailoring examples
- specify how atentication will work
- detail the access control matrix
- define the input validation rules
- choose an error handling and loging approach

***everybody tries to break your app!***

assemble the tam:
- experts in technology
- secrity minded team
- do a high level pentest
- be sure to do root cause analysis on any flaws

how much request our system could have?

how do you control audit data?

desig configuration data for audit 
