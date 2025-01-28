# UAUC Hazard Reporting Solution
## Solution Overview
This Solution is developed to enable staffs identify, report and manage **Unsafe Act & Conditions** in the workplace to enhance safety and prevent accident.

### Key Features:

#### Reporting:

Users can easily report unsafe acts or conditions through a user-friendly interface.
Options to attach photos for better clarity.
#### Categorization:

Reports are categorized based on the type of unsafe act or condition (e.g.,PPE Violation equipment Intergrity,Electrical hazard, Height Related, etc).
Prioritization of reports based on severity and potential impact.
#### Notification:

Automatic notifications to relevant personnel for immediate action.
Follow-up reminders to ensure timely resolution.

#### Tracking and Analytics:

Real-time tracking of reported issues and their resolution status.
Analytics dashboard to identify SBU, Location, and status.
#### Compliance:

Ensures compliance with safety regulations and standards.
Generates reports for audits and safety reviews.

## Solution Justification
Implementing an Unsafe Act/Unsafe Condition application, organizations can significantly enhance workplace safety, ensure compliance, reduce costs, and foster a positive safety culture.

## Solution Taxonomy
Below are the listed order through which this solution was developed, after which each element of the deployment will be documented accordingly.
### Business requirement evaluation.

* Problem review.
* Use case discovery.
* Design conceptualization.
* FitGap Analysis.

## Solution Design
* Data Modelling 
* Security Modelling
* ALM
## Design Approach
* User Interface design 
* The user interface was then transformed using Canvas Apps design object features
* The application functionalities were developed using Power Fx

### Design View
### Canvas Apps Screen
The function used is called the Power Fx, and this was used in various part of the application to achieve the needed behaviours.

       **Home Screen**           

Application User access the platform and by engaging with the "New UA/UC" button can go to the next screen to report hazard observed.

![CanvasApp-Home](https://github.com/user-attachments/assets/7866d26d-4cec-4c39-aa61-91769b825b47)
       
       **UAUC Form Screen**  
       
Application User navigates from the Home Screen to the UAUC hazard reporting form screen and the user is able to submit Observation.

![canvas-form](https://github.com/user-attachments/assets/ed72039b-2407-451a-9c3f-9309ee8adeda)

        **UAUC Edit Screen**  
        
Application User or Action party navigates from the Home Screen (My Submitted UAUC) to the Submitted Hazard form screen and the user is able to edit the "Closed Out Status", optionally attach picture and updates Observation.

![Canvas-Editformform](https://github.com/user-attachments/assets/e89712bf-8960-4d6b-afa4-64137f1bdf01)

       **Gallery Screen**         
##### --Restricted-- 
HSE Team members only can navigate from the Home Screen (HSE Team) to the "All UAUC Hazard Report" Screen to view and also navigete "UAUC Edit Screen".

 ![CanvasGallery](https://github.com/user-attachments/assets/dd19141a-b9b0-4c6d-be3f-0b770769798d)

       **Success Screen**          

Application user is been redirected to success screen if the UAUC form submission was successful.

![SuccessScreen](https://github.com/user-attachments/assets/088350cb-5c35-455f-805e-4609188cbbb8)


       **DashBoard Screen**          


HSE Team members only can navigate from the "All UAUC Hazard Report" Screen to the  to view UAUC Hazard Report DashBoard analytics.

![UAUC DashBoard](https://github.com/user-attachments/assets/8d17d489-f6fb-4f59-bdf1-3aa0db92d96c)

### Data Source  

This table shows the Sharepoint columns for the UAUC solution 

| Columns  |  Type |   
|---|---|
| Unsafe Act / Unsafe Condition (UA/UC) Observed  |  Single line of text |   
| Category of UA/UC Reported  | Multi-Choice  |   
|  Immediate Corrective Action Taken/Further Action Required | Single line of text  |   
|  Action Party | Person or Group  |  
|  RiskRating |  Choice |   
|  Close-Out Status | Choice |  
|  Location | Choice |   
| Observed By  | Single line of text  |  
| Date Of Observation  | Date  |   
| Evidence Attachment  |  Image |   
| Evidence of Closure  |  Image |   
        
        
       Power Automate Cloud Flow      

The image below shows the function written to check if the conditon "Close-out Status" was met after 24 hours.
The function used is called the Power Fx, and this was used in various part of the application to achieve the needed behaviours.

![UAUC Flow](https://github.com/user-attachments/assets/f4074774-9500-457c-b01e-f048865a4a0d)



## Solution Flow Chart

### Canvas App Flow Chart
This chart shows the user journey from process initiation till finish.

![Canvas App Chart](https://github.com/user-attachments/assets/253a227f-444f-4e7e-9d29-86c3f2e4af1c)

### Power Automate Work Flow Chart
This flow charts shows the process model and journey of the implemented automation.

![PA - Work flow](https://github.com/user-attachments/assets/67099e5f-2335-4195-8acd-e6a543cbbc96)



