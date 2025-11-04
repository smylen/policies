# 1. Introduction

Smylen, Inc ("Smylen") is committed to ensuring the confidentiality, privacy, integrity, and availability of all electronic protected health information (ePHI) it receives, maintains, processes and/or transmits on behalf of its Customers. As builders of compliant, hosted software used by health practicioners, consumers, insurance brokers, businesses, and various types of organizations ("Customers"), Smylen strives to maintain compliance, proactively address information security, mitigate risk for these Customers, and assure known breaches are completely and effectively communicated in a timely manner. The following documents address core policies used by Smylen to maintain compliance and assure the proper protections of infrastructure used to store, process, and transmit ePHI for Smylen Customers.

Smylen provides a technology enabled, mobile web based marketplace ("platform") for consumers to book dental treatments, and a membersip rewards program sponsored by organizations and offered to groups. These Categories are cited throughout policies as Customers in each category inherit different policies, procedures, and obligations from Smylen. 

The platform stores dental treatment information and medical history to provide a seamless consumer experience going to the dentist. Smylen makes every effort to reduce the risk of unauthorized disclosure, access, and/or breach of Smylen customer data through the use of secure cloud technologies. Our platorm is locked down at all levels including the network (firewalls, dedicated VPC, etc), server (encryption at rest and in transit, strict of use containers, etc) and application layer. Access is limited to those who need it for their jobs, and any changes or exceptions are documented so such that these claims are verifable by audit. 

## 1.2 Compliance Inheritance

Smylen provides compliant hosted software for its Customers. Smylen is a new company and has not completed a HIPAA/HITRUST compliance audit by a national third-party compliance firm to validate and map organizational policies and technical controls to HIPAA rules. Smylen's CTO has built the company policies, procedures, and technology with HIPAA/HITRUST in mind and is seeking a firm to conduct an audit to verify this claim. Notewistanding, Smylen's platform was built by security and privacy experts, runs entirely on AWS using its highest grade of security tooling; current production systems on AWS will be included in Smylen's third-party audits and HITRUST certification.

Smylen signs business associate agreements (BAAs) with its Customers who are dentists and the covered entitiy. These BAAs outline Smylen obligations and dentist obligations, as well as liability in the case of a breach. Smylen does not manage aspects of compliance for Customers. Certain aspects of compliance cannot be inherited. Because of this, Smylen Customers, in order to achieve full compliance or HITRUST Certification, must implement certain organizational policies. These policies and aspects of compliance fall outside of the services and obligations of Smylen. 

Smylen does not act as a covered entity. When Smylen does operate as a business associate (not a subcontractor), Smylen provides access to ePHI in the platform only to those delivering or recieving treatment.

Smylen signed a BAA with AWS as they manage the security of our infrastructure from datacenter, network up to but not including the application and data. The network, servers, container management, databases and storage are secured by AWS and covered by their BAA. In addition, we use AWS SecurityHub, GuardDuty and CloudTrail for continuous monitoring, remediation and compliance.  

## 1.3 Smylen Organizational Concepts

The entire infrastructure environment is hosted at [AWS](https://aws.amazon.com/). Smylen does not have physical access into the network or server components. The Smylen environment consists of nginx load balancers and web servers; scalable Node.JS application servers; MySQL and Redis database servers; S3 encrypted file storage; Cloudwatch logging and monitoring; Docker containers; and replicated dev/staging environments in seperate AWS account.

Within the Smylen environment on AWS, all data transmission is encrypted and all hard drives are encrypted so data at rest is also encrypted; this applies to all servers - those hosting Docker containers, databases, APIs, log servers, etc. Smylen assumes all data *may* contain ePHI, even though our Risk Assessment does not indicate this is the case, and provides appropriate protections based on that assumption.

In the case of Smylen Customers, it is the responsibility of the Customer to restrict, secure, and assure the privacy of all ePHI data on their end of the wire, as this is not under the control or purview of Smylen.

## 1.4 Requesting Audit and Compliance Reports

Smylen, at its sole discretion, shares audit reports, including its HITRUST reports and Corrective Action Plans (CAPs), with customers on a case by case basis. All audit reports are shared under explicit NDA in Smylen format between Smylen and party to receive materials. Audit reports can be requested by Smylen workforce members for Customers or directly by Smylen Customers.

The following process is used to request audit reports:

1. Email is sent to compliance-reports@smylen.com. In the email, please specify the type of report being requested and any required timelines for the report.
2. Smylen staff will log an issue with the details of the request into the Smylen Task Management System. The Smylen Task Management System is used to track requests' status and outcomes.
3. Smylen will confirm if a current NDA is in place with the party requesting the audit report. If there is no NDA in place, Smylen will send one for execution.
4. Once it has been confirmed that an NDA is executed, Smylen staff will move the issue to "Under Review".
5. The Smylen Security Officer or Privacy Officer must Approve or Reject the Issue. If the Issue is rejected, Smylen will notify the requesting party that we cannot share the requested report.
6. If the issue has been Approved, Smylen will send the customer the requested audit report and complete the Task Management System issue for the request.

## 1.5 Version Control

Refer to the GitHub repository at [github.com/smylen/policies/](https://github.com/smylen/policies/) for the full version history of these policies.
