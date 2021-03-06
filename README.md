
# 18FRFQ-Response
Final Deliverable for 18F Request for Quotation 
=======
[Working Prototype](http://52.1.100.220:8080/jigsaw/#/)

![alt tag](/agile-process-photos/response-images/proposal-header.png?raw=true)

# Request for Quotation 4QTFHS150004 Multiple Award Blanket Purchase Agreement for Agile Delivery Services (ADS I) 

## Introduction
Upon receipt of the RFQ, our team decomposed the RFQ to understand the scope and initial resources required for the effort. The following describes our approach and a bit of the history of this short lived project. We adapted a few agile techniques including Scrum, Kanban, and XP to support this effort.  The basic solution leverages FDA Food Recall Enforcement Reports dataset. The vision of the prototype as an interactive web tool used to inform and educate consumers of food product recalls that are in an open or closed status.
![alt img](/agile-process-photos/design/high-level-overview.png)

## Team 
Extenuating circumstances upon RFQ drop, required us to redefine 100% of our resources. Within 24 hours, our full multidisciplinary team had been assigned, covering eight labor categories -Agile Coach, Visual Designer, Interaction Designer, Back End Developer, DevOps Engineer, Front End Developer, Product manager and Business Analyst.  Our Team’s Corporate reach back helps to address surge and evolving needs by tapping 3,800 US based Agile resources, 1,800 scrum masters and 800 DevOps practitioners. Our proven experience executing Agile processes that has been applied to over 1,000 Agile Scrum, Kanban & Lean projects, spanning Federal & commercial projects, provided the framework and tools to quickly define sprint zero needs, and enable the teams to begin sprinting.  Our team was empowered, self-organized and accountable for delivering value daily within each 'daily' sprint. Although not ideal or typical, our team did not have the luxury of each member dedicating 100% of their time to the RFQ.  Some roles were shared as team members came in and out. With this, it was imperative that the team openly communicate, share dependencies, maintain high visibility, and resolve impediments together.  
## Basic Agile Process 
Due to the very short turn around we took a modified agile management approach based on Scrum and Kanban leveraging a [physical task board](agile-process-photos/process-photos/6.18.2015 14.03 - kanban board.jpg). We had daily 'sprints' where we had a [team stand-up](agile-process-photos/process-photos/6.19.2015.0907 - standup.jpg) in the morning to understand where each team member was regarding what had been completed, what was to be worked on next, and any issues/impediments that was of concern. This kept all the tasks very visible, lightweight, fast moving, and easy for all to see the current state of the project.  Each afternoon we had a sprint review where the team met to review the progress made for the day and begin [planning](agile-process-photos/process-photos/2015-06-29 09.18.32 - work-in-progress.jpg) for the next day's sprint.  Once new stories, features, defects, functionality or change requests had been captured via stickies on the task-board, the product owner would prioritize the backlog based on user impact, time and value. This prioritization enabled the PO during our daily sprint planning to set the sprint goals, and allow the team to define how those goals would be implemented and what could be taken on during the sprint.    
##Human Centered Design 
Human Centered Design stood as the backbone of our prototype. The end user desiring information pertinent to FDA Food Recalls, their needs, wants and desires drove a prototype tailored uniquely to them.  The following summarizes our basic approach. 

1. Understand User Context. Three personas were developed to depict multiple user bases for the prototype. 
 1. Ann Jordan a Mom searching for information for her children 
 2. Steven Jones an FDA Administrator monitoring site metrics and updating public information 
 3. Kathy Miller a Nutritionist looking for update for her client base 
2. [User stories](agile-process-photos/process-photos/2015-06-26 09.52.14 - backlog.jpg)  with acceptance criteria were defined to help understand end-user aspirations.  We conducted an end-user survey at a local grocery store with four people matching our Personas to further understanding.  PO engagement ensured their requirements were incorporated.   Our personas described a need where the solution had to be versatile, responsive, interactive and seamlessly support a variety of end-user devices.  Using responsive design techniques, the UX designers focused on crafting each targeted device to provide optimal viewing and interactive experiences. Users are presented different layouts based on devices and content also adapts to specific device types and its orientation.  Users of higher resolution devices are presented with appropriate content.  Mobile users will be presented with content and layout more appropriate for limited real estate and quick access to critical information.    
3. Once our understanding evolved, rapid prototyping allowed for [design iterations](agile-process-photos/process-photos/wireframe (added 6.23).png) and quick changes driven by continual feedback from the PO, usability and 508 testing, surveys and the team.  Stories were created and prioritized to ensure the most valued work was addressed to respond to user needs.  
4. We conducted usability testing with local/remote testers along with remote observers using COT usability tool Morae allowing collaboration between test administrators and remote observers. 508 and accessibility testing using JAWS screen reader, the WAT toolbar and Keyboard Accessibility helped drive continuous improvement and enhance usability for disable users.   


## Design Style Guide 
Our user first focus leveraged pattern libraries (e.g. Font Awesome, Bootstrap) and a lightweight design guide to drive the UX and design patterns to help maintain a consistent user experience among our designers and across multiple devices.  Bootstrap was used to develop our multi-device framework.  This encouraged collective code ownership, making it easier for our developers to work across the code base.  The team had two UX designers, one remote and one onsite with the team.  Developing and implementing Pattern libraries and UI libraries also allowed the team to have functionality and design elements that could be reused, and compliant with 508, keeping cost and time at a minimum.  
## Testing 
Unit Tests - For the backend unit testing we utilized JUnit and Spock.  All components received unit tests, especially corner cases and null.  Unit tests were created simultaneously as code was developed. Unit tests *(NUMBER OF TESTS) * were run on every Jenkins build  (NUMBER OF BUILDS).  If defects and or bugs were identified, the developer would resolve the defect within the same sprint.  No known defects were identified that were handled out of the sprint boundary.   
Usability testing was implemented in a series of steps.  Multiple iterations were created through moc-ups and wire frame development. At the daily sprint review, designs were reviewed and feedback from the development team, product owner and stakeholders was incorporated to subsequent designs. Within 48 hours of the initial product direction a solid design was conceptualized in an interactive, clickable wireframe. In 72 hours, [usability test cases](process-video/Alison usability test.mp4) were created and testing was administered with real users against that design with individuals who matched the personas created for the prototype. Local and remote testing was conducted. Based on feedback received, the designs were refined and iterations made.  
[508 testing](process-video/508-testing.MOV) was done utilizing JAWS, the Wat toolbar and Keyboard Accessibility. Results highlighted areas of our implemented design were not conducive to individuals with disabilities. These critical tests allowed our team to ensure our prototype vision was accessible for all users.    
## Technology Choices 
Open source technologies allowed our team to drive efficiencies through cost, time, reliability and value.   The underlying platforms used in our prototype are openly licensed and free.  A complete list of tools used can be found here: PLACE URL HERE 
![alt tag](/agile-process-photos/design/tool-diagram.png)

## Development 
1. Used 4 API's (List them)  
2. UCD drove API's (List them)  
3. Front end development drove APIs (List them) - front end developers produced the spec's and the backend developers created the working API', as identified.

The team both provided and consumed a RESTfull API (List them).  Development dependencies across layers of the architecture was mitigated by first creating a shell end-point available to begin to integrate with.    Developer review and interaction with the shell end-points results in feedback and resulting changes.  Ultimately a final API is established with appropriate unit tests are committed for build.  Our API's enriched the data set by normalizing state recall information that was embedded in the free text.  A specific data element was added to easily represent the formal list of states associated with the recall.  
The team utilized Github for configuration management. Three backend developers each worked part time, to ensure continuity and CM best practices they used Github time stamps and the check in-check-out feature to work on the most recent code sources.  The team built in the ability to trace any warfile back to the Jenkins Job/Build and commit reference in Github. This allowed tractability and a testing reference for each build.  

## Deployment 
Deployed to AWS - Need follow up here. AWS IaaS with Jenkins deploying to Tomcat (Describe the deployment process and ultimate IaaS environment)  
![alt tag](/agile-process-photos/design/deploy-stack.png)

1. Docker, explain why we used docker ?(Sean & Josh EXPAND) 

Continuous Monitoring 
To provide continuous monitoring the team developed an administrative view to a dynamic page. This url is not accessible from the main page but is available here: http://52.7.254.19:8080/jigsaw/#/appMetricsMetrics .   This monitoring app is just a start to provide insight into the activity of the application and to monitor for intrusions, denial of service attacks, etc.  Since we chose to use only publicly available data and do not require any authentication, there is no need to store any end-user sensitive information.  These choices were intentional to lower the security profile.  Clearly a full security assessment is in order as this solution moves to production.  

## Conclusion 
All of our evidence is in this Git repository and can be leveraged as needed.  Click here for our [evidence summary](evidence)


