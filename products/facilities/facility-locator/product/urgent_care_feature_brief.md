
# _Facility Locator Urgent Care redesign Feature Brief_

This document will focus on the MVP for the Facility Locator UX redesign: Community Care/Urgent Care. 
## Table of Contents
[User Journey](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/facilities/facility-locator/product/urgent_care_feature_brief.md#user-journey)
[User Stories](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/facilities/facility-locator/product/urgent_care_feature_brief.md#user-stories--use-cases)
[Project Rationale](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/facilities/facility-locator/product/urgent_care_feature_brief.md#project-rationale)
[Project Scope and Scale](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/facilities/facility-locator/product/urgent_care_feature_brief.md#project-scope-and-scale)
[Not in Scope](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/facilities/facility-locator/product/urgent_care_feature_brief.md#not-currently-in-scope)
[Measuring Success](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/facilities/facility-locator/product/urgent_care_feature_brief.md#measuring-success)
[Dependencies](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/facilities/facility-locator/product/urgent_care_feature_brief.md#dependencies)
[Risk factors](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/facilities/facility-locator/product/urgent_care_feature_brief.md#risk-factors)
[Rejected Solutions](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/facilities/facility-locator/product/urgent_care_feature_brief.md#rejected-solutions)
[Definition of Done](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/facilities/facility-locator/product/urgent_care_feature_brief.md#definition-of-done)
[Key Links](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/facilities/facility-locator/product/urgent_care_feature_brief.md#key-links)

### User Journey
- Following the Mission Act, eligible Veterans have access to urgent care benefits in their community and need help knowing where and how to receive care. 

### User Stories / Use Cases
*What two or three core use cases do we believe should cover ~80% of users?*
- As a Veteran using the Tricare or Optum network area, I need to...
  - Find the appropriate urgent care facility for my situation so I can use my benefits for care.
  - Find a retail pharmacy so that I can have fill my prescription. 
  - Understand my available benefit so I can be prepared for my visit to the urgent care/retail pharmacy.

### Project Rationale
_Why should this project be a priority?_ 
- The current implementation is not consistent with Veterans' mental models for urgent care. 
- The separate TriWest facility locator leads to a misunderstanding of coverage for the returned providers.
- The current implementation considers only TriWest network providers.  
- Users don't have a easy way to search for urgent care facilities.

**Stakeholder/Business drivers**
- The Office of Community Care has been dissatisfied with the community care implementation. 
- Urgent care is a particularly high visibility subset of Community Care functionality. Searches continue to be directed to an external TriWest Provider locator due to Veteran confusion and data quality concerns. 
- The impending addition of the Optum network of providers on 2/1/2020 increases the priority of this work. 

**Findings from research conducted December 2019**
- Veterans are not aware of the type of care they can receive at urgent care facilities. There is a general lack of communication/education around the difference between community care providers and VA health care
- When prompted to choose an urgent care location to stitch a wound, a majority of participants mentioned that they would visit an ER or VA facility and not an Urgent Care location.
- Participants were drawn to location input and dropdowns and did not choose to filter their search results.
- Overlapping benefits cause confusion when visiting in-network providers.
- Internal language and inconsistent labeling cause users to hesitate when looking into facilities.
- Participants did not understand the difference between "retail" urgent care and urgent care until they were given a definition and example treatments

### Project Scope and Scale
_What's in and what's out?_
**MVP**
- Iteration incorporates previous community and urgent care research, Facility Locator discovery research and feedback
- Veterans are assisted in understanding the sub-type choices for urgent care and are able to determine which facility type meets their current need.
- Veteran can differentiate between urgent care sub-type in search results (but do not necessarily need to be able to filter or search by sub-type in MVP)
- Facilities returned as results of urgent care search do not reference a need for referral. [#4241]
- Veterans have easy access to the PDF (or a placeholder) explaining the urgent care benefit.
- Workflow includes information to help the Veteran understand how to fill an Urgent Care Pharmacy Prescription
- Design does not include TriWest link (which will be removed pending OCC approval)

**MVP will also include some general usability and search functionality improvements**

Focused on solving the following problems:
- Search UI is inconsistent (i.e., free text search box, dropdowns, typeahead)
- Map functionality is confusing (iconography, results, mileage)
- Search parameters for facility type/service is not consistent with Veterans' mental models about care.

To address the following user stories: 
- As a Veteran, I want reliable and consistent information between online and physical locations so that I can trust the information which is displayed. 
- As a Veteran, I need multiple entry points to the Facility Locator tool so that I can search for a facility from different Va.gov hubs.
- As a Veteran, I want to view high level location information included with the search results (ie: Phone number, Today's hours. Directions, Service selected)

**Future Iterations for Community Care/Urgent Care**
- Veteran may need to filter/search based on urgent care sub-type. (Will be informed by future research)
- Workflow iterations for urgent care prescriptions

### Not currently in scope
- Emergency care
- Remaining Community Care services

### Measuring Success
_How will we know if we are successful?_
**Objective: Reform Community Care Implementation**
  - Key Result #1: The rate of search refinements for Community Care will be at parity with VA facility searches by July 1, 2020. 
  - Key Result #2: All urgent care searches will be performed using the modernized Facility Locator by February 2, 2020.  

### Dependencies
_Are other features dependent on this one? What do we need from partners? What do we need outside of engineering?_
**Team/Internal dependencies**
  -  Ability to differentiate among facility sub-types is access dependent.
  - Comprehensive QA strategy requires lower environment with PPMS data for testing. 
  
**Partner dependencies**
  - Data quality is dependent on data owners, in part. (PPMS)
  - Benefit PDF will be available, pending OCC approval. 
  
  ### Risk factors
  - This UX redesign is reliant on the data provided via PPMS and is dependent on the resolution of existing data concerns.
  - This work is dependent on the availability of Optum network information.

### Rejected Solutions
*What other approaches did we consider and why were they rejected?*
- Considered the need to return emergency care as part of urgent care research results
  - Emergency care will be separate facility type 

### Definition of Done
- The Veteran must be able to successfully search for an urgent care facility.
- The Veteran must be able to successfully search for a retail pharmacy.
- High level location information is included in search results.
- The Veteran can view the name, address, phone number, directions, hours of operation and services offered for the chosen facility. 
- The Veteran can download benefit information to take to the facility.
- Veterans using assistive technology can achieve the stated goals above.  
- Existing functionality for searching VHA(including Vet Centers), VBA and NCA facilities will be maintained. 

### Key Links
_Links to requirements documentation, wireframes/mock-ups, research, etc._








