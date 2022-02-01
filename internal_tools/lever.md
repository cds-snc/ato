---
name: "Lever Hire Applicant Tracking System"
status: "Complete"
date_requested: "2019-01-04"
date_approved: "2019-01-25"
approved_by: "John O'Brien, Anatole Papadopoulos, Paul Girard"
---

# Lever Hire Applicant Tracking System

## General information

**System name:** Lever Hire Application Tracking System

**Date:** 2019-01-04

**Document classification:** Unclassified

## Purpose

This report documents the residual risk associated with operating the Lever Hire **Applicant Tracking System**. It documents the accountability, approvals and Risk Management signatures that are required to authorize this system for operation.


## Background

The Canadian Digital Service (CDS) was launched in July 2017. It has a mandate to improve the quality of digital services the Government delivers to Canadians, by partnering with federal departments to design and build services using modern technology best practices, user research, and software development techniques. A core part of CDS’s role is to bring world-class digital professionals into the public service for tours of duty.

CDS’s rapid growth and multidisciplinary hiring has presented a number of logistical challenges for its Internal Operations team, from recruitment and screening to classification processes. More than 50 new (largely external) staff have joined CDS in the year since launch. More than 1600 applications have been received since CDS opened its general recruitment form in September 2017. In order to successfully manage this level of interest, better tools are needed to ensure the integrity and quality of CDS’s recruitment process. Currently, applicants submit an initial expression of interest through the CDS website. Their submission is sent to a recruitment specific mailbox on the TBS corporate exchange server. Staff continue the process by manually transferring the information into an Excel spreadsheet and managing the process in this very time-consuming approach.


## System information

CDS plans to implement an **Applicant Tracking System**, based on research from the Internal Operations team and best practices from the technology industry (including recommendations from Shopify and other Canadian technology leaders). In line with the GC’s Cloud Adoption Strategy, which recommends the public cloud deployment model and the software-as-a-service (SaaS) delivery model, CDS is planning to move forward with a SaaS-based Applicant Tracking System hosted on public cloud. 

The Applicant Tracking System will:

* provide a better user experience for candidates for CDS positions; 
* protect applicant data by standardizing its handling; and 
* enable the CDS talent team and hiring managers to work seamlessly together to ensure applications are managed promptly and consistently.

In accordance with the Statement of Sensitivity, the data that will be processed and stored in the Lever Hire platform has a security category of Protected A. 

## Technical information

Lever Hire is a web application that is accessible through a web browser. It provides an online interface for external applicants to apply, and a comprehensive online interface for hiring staff to review, assess, and categorize applicants.

For external applicants, Lever Hire provides an application form for each role, that can be customized and branded by the organization. This allows applicants to input their contact details, hiring criteria, etc. as well as upload a CV, portfolio, or other accompanying documents.

Lever Hire is a SaaS product hosted on the Amazon Web Services public cloud in the US-West region. Lever, as a SaaS provider, is responsible for both the security of their application and the cloud infrastructure leverages. As a consumer, CDS is responsible for the secure use and configuration of the service. 

Lever Hire uses AWS infrastructure spread across multiple availability zones, and has a dedicated information security team and intrusion detection tools in place to monitor its systems. AWS is one of the approved cloud service providers (CSP) in the GC under the current Unclassified cloud vehicle. AWS has also onboarded to the CSE CSP IT Security Assessment program and has been assessed based on the GC Security Control Profile for Cloud-based Services at the PBMM level.  

Lever has provided two confidential SOC 2 Type 2 reports, completed by a third party auditing firm, detailing its organizational and security practices, including detailed monitoring of technical systems, limitation of privileges, and staff security and ethics training.

The security controls that CDS is responsible for are [relatively small](https://docs.google.com/spreadsheets/d/1bvFjutaYJBHueGrwnpr3JxW_btNJEChpSZj2olEAtZI/), due to the benefits of using a SaaS-based offering. The following are some measures that CDS is taking to ensure that the service is used securely:

* Only CDS staff with authority to access HR information will have accounts to the Lever Hire platform. Staff will use either their corporate TBS devices or the managed CDS MacOS devices with appropriate security controls enforced through the Jamf device management solution. For example: full hard drive encryption (SC-28), remote wipe (MP-6 (8)), password-based authentication management (IA-5 (1)). This Jamf device management project is ongoing and targeting the CIS benchmarks. 
* All access to the Lever Hire platform requires mandatory two-factor authentication, backed by hardware based YubiKeys that support Universal 2nd Factor (U2F).
* CDS has adopted a continuous monitoring approach for monitoring its vendors. This includes ongoing use of a security rating services (BitSight), planned escalation and incident response processes, and security scenario exercises. 

**Evidence used as input to this assessment:**

<table>
  <tr>
   <td><strong>Statement of Sensitivity</strong>
<p>
2018-10-25 Recruitment Security Categorization - CDS ATS.xlsx
   </td>
   <td><strong><a href="https://docs.google.com/spreadsheets/d/1bvFjutaYJBHueGrwnpr3JxW_btNJEChpSZj2olEAtZI/">Security Control Traceability Matrix</a></strong>
   </td>
   <td><strong>System architecture / Design Document</strong>
<p>
<a href="https://docs.google.com/document/d/1Nit7sTLg5wUnqyu2y_Nkxpigf4TZBd6qOF3nPZVFhqI/edit">Lever Hire – CDS Recruitment Concept of Operations</a>
   </td>
  </tr>
  <tr>
   <td><strong>Concept of Operations</strong>
<p>
<a href="https://docs.google.com/document/d/1Nit7sTLg5wUnqyu2y_Nkxpigf4TZBd6qOF3nPZVFhqI/edit">Lever Hire – CDS Recruitment Concept of Operations</a>
   </td>
   <td><strong>Security Inputs</strong>
<p>
GC ESA Security Design Patterns for SaaS-based Solutions used as reference model (GCDOCS #33653594).
   </td>
   <td><strong>Security Plan</strong>
<p>
<a href="https://docs.google.com/document/d/1f3aDjMatTvChq30glwgyJeSxOBGH2tMJ5a3xjD3KA7I/edit">Lever Hire – CDS Security Procedures</a>
   </td>
  </tr>
  <tr>
   <td><strong>Security Testing Results</strong>
<p>
bitsight-technologies-company-overview-lever-inc-2018-10-26.pdf
<p>
bitsight-technologies-nist-csf-report-2018-10-26.pdf
   </td>
   <td><strong>Standard operating procedures</strong>
<p>
<a href="https://docs.google.com/document/d/1f3aDjMatTvChq30glwgyJeSxOBGH2tMJ5a3xjD3KA7I/edit">Lever Hire – CDS Security Procedures</a>
   </td>
   <td><strong>Business Impact Assessment</strong>
<p>
<a href="https://docs.google.com/document/d/1Nit7sTLg5wUnqyu2y_Nkxpigf4TZBd6qOF3nPZVFhqI/edit">Lever Hire – CDS Recruitment Concept of Operations</a>
   </td>
  </tr>
  <tr>
   <td><strong>Privacy Impact Assessment</strong>
<p>
Signed PIA Checklist - CDS applicant tracking system.pdf
   </td>
   <td><strong>Third Party Assessment(s)</strong>
<p>
bitsight-technologies-company-overview-lever-inc-2018-10-26.pdf
<p>
bitsight-technologies-nist-csf-report-2018-10-26.pdf
<p>
Lever - 2017 - Type 2 SOC 2 - Report (Password Protected).pdf
<p>
AWS PBMM Assessment - CSE Report
   </td>
   <td><strong>Expired / Previous Security Assessment</strong>
<p>
Not applicable 
   </td>
  </tr>
</table>

## Security Review 

The security review for CDS’s use of the Lever Hire platform does indicate deficiencies in the overall security posture (see action items). However the overall security posture (38/45 security goals met or partially met) demonstrate a strong commitment to security; and CDS’s means of monitoring the Lever Hire platform for decay in its security posture is satisfactory. 

The security deficiencies posing the most risk to CDS are related to contingency planning, data protection and compliance risk. 

Contingency Planning

* Currently the Lever Hire contingency plan and exit strategy have not been exercised. The risk that the contingency plan is only theoretically possible could impact the recruitment business activity with a loss of data and availability. See contingency planning action items below (CP-2, CP-4).

Data Protection



* Currently the disposal procedures for data collected by CDS’s use of the Lever Hire service are insufficient. CDS data within the Lever Hire platform should be kept to a minimum, where possible, in order to minimize the impact of a data breach. See data protection action items below (MP-6 (1)). 

Compliance Risk



* Lever integration with CDS’s G-Suite calendar and contacts will be enabled to ensure the team has an efficient way of scheduling interviews and outreach activities. As part of the SSC cloud contract, Google provided ISO27001 & SOC 2 Type 2 reports. CDS has not yet completed a security assessment of G-Suite. Assessment work for this SaaS product is underway, and expected to be completed shortly (CA-2, CA-6).
* The Apple MacBooks used at CDS are currently not authorized to process Protected A data. It is expected that these assets will be used to access the Lever Hire platform. As a result Protected A information is likely to be cached on these assets. It should be noted that all CDS devices are managed through the use of the Jamf Pro device management tool, and have audit compliance in place based on the CIS Benchmarks, including enforced full disk encryption, remote wipe, strong password policies, and endpoint detection and response (EDR) products are installed. Assessment work for these devices is underway, and expected to be completed shortly (CA-2, CA-6).
* CDS is using the AWS Cloudfront and Lambda platforms to pass applicant data from the CDS website to the Lever Hire platform via their API. As part of the SSC cloud contract, AWS provided ISO27001 & SOC 2 Type 2 reports. CSE has completed their assessment against the PBMM controls, as part of SSC’s ongoing Protected Cloud RFP. Assessment work for our usage of the platform is underway, and expected to be completed shortly (CA-2, CA-6).


## IT Security Recommendations:

At this time, it is recommended that Lever Hire and the services required to operate the platform (AWS Cloudfront and Lambda, CDS Apple MacBooks, G-Suite) be granted an Interim Authorization to Operate for processing and storage of the PROTECTED A data as described in the concept of operations.


## Terms of this Agreement:

The following action items shall be addressed and documented by CDS and progress reported monthly to the CDS Head of Security and Head of Talent.


### Contingency Planning Action Items:



* Develop a contingency plan within the next 3 months (CP-2).
* Exercise the full contingency plan within the next 6 months (CP-4).


### Data Protection Action Items:



* Define procedures for removing unneeded data from the Lever Hire platform within the next 3 months (MP-6 (1)).
* Pipe all external inputs (resumes, links, etc.) through GC controlled file scanning engines to further defend against malicious document attacks within the next 6 months (SI-3).


### Compliance Risk Action Items:



* Complete the security assessment and authorization process for both G-Suite, the Apple MacBooks, and AWS within 12 months (CA-2, CA-6). 