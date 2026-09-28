# 💻 Software Access Management -- ServiceNow

## 📌 Project Overview

**Software Access Management** is a custom ServiceNow application
designed to allow employees to request access to software and
development/testing tools through the **Service Catalog and Service
Portal**.

The application provides a structured request experience where users can
enter employee information, security/access requirements, email details,
and software selections. The solution also uses catalog configuration,
client-side logic, UI policies, and Flow Designer automation to process
requests efficiently.

This project demonstrates practical ServiceNow development skills across
**Service Catalog, Service Portal, Catalog Client Scripts, Catalog UI
Policies, Variable Sets, Variables, and Flow Designer**.

------------------------------------------------------------------------

## 🎯 Project Objectives

-   Create a centralized software access request process.
-   Provide a user-friendly request interface through Service Portal.
-   Collect required information using catalog variables.
-   Organize reusable variables through Catalog Variable Sets.
-   Dynamically control the catalog form using Catalog UI Policies and
    Client Scripts.
-   Automate request processing using Flow Designer.
-   Package the complete configuration using ServiceNow Update Sets for
    deployment.

------------------------------------------------------------------------

## 🖥️ User Interface

The Software Access catalog item is available through the **Service
Portal**.

Users can navigate through the Service Catalog and open the **Software
Access** request form.

### Software Access Catalog Item

The catalog item contains:

-   Requester Name
-   Security Operations information
-   Employee information
-   Company Email
-   Software Selection
-   Additional request information

The request page also provides a clear **Submit** action for users.

![Software Access Catalog Item](screenshots/software-access-portal.png)

------------------------------------------------------------------------

## 🧩 Service Catalog Components

### 1. Catalog

Created a dedicated catalog structure for software-related services.

### 2. Catalog Item

Created a custom **Software Access** catalog item for requesting access
to required software and development/testing tools.

### 3. Catalog Variables

Created variables to capture information required for processing the
software access request.

Examples include:

-   Requester Name
-   Company Email
-   Software Selection
-   Employee information
-   Security Operations information

### 4. Catalog Variable Sets

Reusable variable sets were created to group related variables and
simplify catalog item configuration.

Example groups:

-   **Security Ops**
    -   Actions
    -   Data Sensitivity Level
    -   Required Admin Access
-   **Employee Information**
    -   Employee ID
    -   Department Name
    -   Job Role

![Catalog Variable Sets](screenshots/software-access-variable-sets.png)

------------------------------------------------------------------------

## ⚙️ Catalog UI Policies

Catalog UI Policies were configured to control the behavior and
visibility of catalog variables based on request conditions.

They can be used to:

-   Show or hide fields
-   Make fields mandatory
-   Make fields read-only
-   Control the user experience dynamically

This helps ensure that users provide the appropriate information during
the request process.

------------------------------------------------------------------------

## 💻 Catalog Client Scripts

Catalog Client Scripts were implemented to add client-side logic to the
Software Access request form.

They can be used to:

-   Validate user input
-   Dynamically populate fields
-   Change field behavior
-   Display or hide information based on user selections
-   Improve the overall catalog form experience

------------------------------------------------------------------------

## 🔄 Flow Designer Automation

A Flow Designer flow was created to automate the processing of Software
Access requests.

### High-Level Process

``` text
User submits Software Access request
              ↓
        Catalog Request
              ↓
        Flow is triggered
              ↓
     Request information processed
              ↓
   Required actions / assignments
              ↓
       Request processing
              ↓
          Completion
```

The flow helps reduce manual processing and provides a structured
approach for handling software access requests.

------------------------------------------------------------------------

## 🌐 Service Portal

The project uses **Service Portal** as the user-facing interface.

Users can:

-   Browse the Service Catalog
-   Locate the Software Access service
-   Enter request information
-   Submit the request
-   Track submitted requests

------------------------------------------------------------------------

## 📦 Update Set

The project configuration has been captured in a **ServiceNow Update
Set**.

The Update Set contains the configuration required to move the
application between ServiceNow instances.

### Deployment Steps

1.  Open the target ServiceNow instance.
2.  Navigate to:

``` text
System Update Sets → Retrieved Update Sets
```

3.  Import the provided Update Set.
4.  Open the Update Set.
5.  Click **Preview Update Set**.
6.  Review and resolve any preview errors.
7.  Click **Commit Update Set**.
8.  Verify the Catalog, Variables, Variable Sets, UI Policies, Client
    Scripts, Service Portal experience, and Flow.

------------------------------------------------------------------------

## 🧠 ServiceNow Concepts Demonstrated

This project demonstrates hands-on experience with:

-   Service Catalog
-   Catalog Items
-   Catalog Variables
-   Catalog Variable Sets
-   Catalog UI Policies
-   Catalog Client Scripts
-   Service Portal
-   Flow Designer
-   Request Management
-   Form Configuration
-   Client-side Automation
-   Workflow Automation
-   Update Sets
-   ServiceNow Application Development

------------------------------------------------------------------------

## 📁 Project Structure

``` text
Software-Access-Management/
│
├── README.md
├── Update-Set/"
│   └── software-access-management.xml
│
└── screenshots/
    ├── software-access-portal.png
    └── software-access-variable-sets.png

------------------------------------------------------------------------

## 🚀 Future Enhancements

Possible enhancements include:

-   Approval workflow for software access requests
-   Automated email notifications
-   Integration with software/license inventory
-   SLA configuration
-   Manager approval
-   Access expiration and renewal
-   Reporting and dashboards
-   Integration with external identity/access-management systems

------------------------------------------------------------------------

## 👩‍💻 Author

**Rani Mahadev Pujari**

ServiceNow Developer \| Data & AI Enthusiast

------------------------------------------------------------------------

## 📌 Project Status

✅ Custom ServiceNow application created\
✅ Service Catalog configured\
✅ Software Access Catalog Item created\
✅ Catalog Variables created\
✅ Catalog Variable Sets created\
✅ Catalog UI Policies configured\
✅ Catalog Client Scripts implemented\
✅ Service Portal interface configured\
✅ Flow Designer automation created\
✅ Update Set created and uploaded
