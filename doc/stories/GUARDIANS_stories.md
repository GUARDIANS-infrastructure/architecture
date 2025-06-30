## Motivation

This is an opinionated first take on some important user stories for a national human omics research data infrastructure. It is meant to reflect work that partners are currently engaged in, identify generic common uses, and suggest future sources of value. It serves to demonstrates one approach to analysis and diagramming. It also aims to foster alignment among partners by highlighting program scope, shared interests, and opportunities for collaboration. Important caveats:

* This is absolutely not an exhaustive list, ‘The top 25’, or even ‘Our top 25’ in importance.

* There are varying levels of granularity here. Some are epic-level system stories. Some are nearly feature-level user stories. 

* We’ve taken a maximalist interpretation of the concept of ‘user’: as someone that interacts with the system in some capacity [\[1\]](?tab=t.0#bookmark=id.roq4hcx5yo20). Importantly, this includes the design, development, and operation of systems as well as ‘consumer-level’ interactions.

---

## Twenty-five user stories

1. *As a* **researcher**,  
   I browse a catalog of Australian-held human omics datasets, *so that*  
   I may understand the landscape of available data.[^1]

2. *As a* **researcher**,  
   I view a high-level description of a dataset of interest, its conditions for use, and where it is held, *so that*  
   I may understand the dataset and how to apply for access.

3. *As a* **researcher**,  
   I access a service using credentials provided by my Australian research organisation, *so that*  
   I may apply for access to a dataset.

4. *As a* **researcher**,  
   I apply for access to a dataset within a Trusted Research Environment (TRE), *so that*  
   I may use the TRE to analyse the data there.

5. *As a* **researcher**,  
   I apply for access to a **compute resource**, *so that*  
   I may use the resource to analyse data that I will provide.

6. *As an* **authorized data user** granted ‘get’ access to a dataset,  
   I fetch the data to an environment of my choice, *so that*  
   I may analyse the data there.

7. *As an* **authorized data user** granted ‘in-situ’ access to a dataset in a TRE,  
   I use the tools within the TRE, *so that*  
   I may analyse the data there.

8. *As an* **authorized[^2]** **researcher**,  
   I access a general-purpose compute environment, *so that*  
   I may analyse data that I provide, using tools available in the environment.

9. *As an* **authorized** **researcher**,  
   I access a managed workflow service, *so that*  
   I may analyse data that I provide, using workflows available in the service.

10. *As an* **authorized** **researcher**,  
    I access a custom omics analysis platform, *so that*  
    I may analyse data that I provide and/or that exists within the platform.

11. *As a* **data owner**,  
    I implement in policy the current guidance on the Australian ELSI landscape around human omics data sharing, *so that*  
    systems and processes I am responsible for do comply with law, regulation, and community expectations

12. *As a* **data owner**,  
    I store my data in a repository within Australia, managed by a trusted **data custodian**, *so that*  
    valuable human omics datasets may be shared responsibly with **authorized data users**.

13. *As a* **data owner** (or delegate),  
    I review, approve or reject a dataset application, *so that*  
    I may control authorization of **data user** access to the data managed by a trusted **data custodian**.

14. *As a* **data owner** (or delegate),  
    I get a report of currently **authorized data users** of my data, and a record of all applications, *so that*  
    I may fulfil my oversight responsibilities and demonstrate the value of the data.

15. *As a* **data steward**,  
    I describe and annotate my datasets using standard ontologies, *so that*  
    valuable human omics datasets are findable and meaningful to **data users**.

16. *As a* **data steward**,  
    I provide my data in standard data structures and file formats, *so that*  
    valuable human omics datasets are useful to **authorized data users**.

17. *As a* **data steward**,  
    I implement the **data owner’s** policies regarding appropriate use of data systems and **data users**’ data, *so that*  
    systems and processes I am responsible for do comply with policy, minimizing the likelihood and impacts of misuse.

18. *As a* **data custodian** (access control),  
    I maintain a definitive, current record of which **data users** have been approved by **data owners** to access which datasets, *so that*  
    **data custodians** (holders) may access a single, secure point of truth for authorization.

19. *As a* **data custodian** (access control),  
    I implement controlled access to datasets for **data users** on behalf of a **data owner**[^3] *so that*  
    **data owner** decisions about access (deny, grant, revoke) are represented in an accurate and timely fashion.

20. *As a* **data custodian** (holder),  
    I hold data on secure storage systems under local jurisdiction, on terms mutually agreed with **data owners**, *so that*  
    valuable human omics datasets are available for appropriate re-use by Australian researchers.

21. *As a* **data custodian** (holder),  
    I provide low-latency, high-bandwidth access to human omics data for **authorized data users** via standard mechanisms and protocols, *so that*  
    valuable human omics datasets are accessible using standard tools, with minimum delay.

22. *As a* **compute resource provider**,  
    I review, approve or reject an application for access to **compute resources**, *so that*  
    I may control authorization of **researcher** access to the compute resources I manage.

23. *As a* **compute resource provider**,  
    I track system resource use at the **researcher** level, *so that*  
    I may generate cost reports.

24. *As a* **clinical research coordinator**,  
    I generate a report on the number and current consent status of participants in a trial, *so that*  
    I may fulfil my oversight responsibilities and track enrollment progress.

25. *As a* **provider of web services and APIs**  
    I describe the endpoints I host using standard protocols *so that*  
    endpoints may be aggregated together to form catalogues and networks of services

---

## Glossary

| Authorized | Granted conditional permission to use a resource (data or compute) |
| :---- | :---- |
| **Clinical research coordinator** | A Clinical Research Coordinator (CRC) manages and conducts the day-to-day activities of a clinical trial. |
| **Compute resource**  | For example: an analysis platform, managed workflow service, or general-purpose compute environment. These resources may be distinguished by: in-theory unbounded resource requirements of single-user jobs, and/or non-linear marginal cost to supply additional demand. For example, an online catalog service is not a compute resource. |
| **Compute resource provider** | Provider or administrator of a compute resource. Whether on-prem or in the cloud, ultimately they foot the bill — which may or may not be passed on to users. |
| **Data custodian[^4]** | A role responsible for one or more aspects of safe custody, transport and storage of data, and implementation of business rules and/or the technical environment to control access. Job titles with some data custodian responsibilities may include system administrator, database administrator, dev/ops or data engineer. |
| **Data steward** | A role responsible for ensuring data quality and fitness for purpose of the organization's data assets, and for implementation of governance. They ensure data quality, accuracy, and adherence to business rules and policies. |
| **Data owner[^5]** | The legal person, agency, or body that has authority and is accountable for their organisation’s data and may delegate responsibilities to a Data Steward. They have the authority to make decisions about data usage, access, and governance. |
| **Data user** | An individual or group that accesses and uses data for various purposes, such as research. |
| **General-purpose compute environment** | e.g. HPC, low-level cloud compute services e.g. AWS EC2, Batch |
| **Managed workflow service** | e.g. Seqera, Terra |
| **Researcher** | A (potential) consumer of the data and/or compute resources available in the ecoystem |
| **Trusted Research Environment** | A compute environment set up for research with sensitive data that has built-in security controls and user access management features. The [SARTRE](https://satre-specification.readthedocs.io/en/stable/faqs.html#what-tre) spec has detailed guidance on what constitutes a TRE. |

---

![internal personae](../../diagrams/GUARDIANS_all_internal.svg "Internal Personae")

![all](../../diagrams/GUARDIANS_all.svg "All")

![journey 1](../../diagrams/GUARDIANS_researcher_journey_1.svg "Journey 1")

![journey 2](../../diagrams/GUARDIANS_researcher_journey_2.svg "Journey 2")

---

## An aside: on symmetry

Thinking about user stories in pairs can reveal system-wide patterns and gaps. For every **consumer story** — someone using the system to achieve a goal — there’s a complementary **producer story** describing the people or processes that make that functionality possible. For example:

1. *As a* **researcher**,  
   I browse a catalog of Australian-held human omics datasets, *so that*  
   I may understand the landscape of available data.

2. *As a* **data steward**,  
   I describe and annotate my datasets using standard ontologies, *so that*  
   valuable human omics datasets are findable and meaningful to **data users**.

These aren’t perfect mirrors. **Consumer stories** usually follow the pattern:  
*User uses feature → to achieve their own outcome*

whereas **producer stories** tend to be:  
*User builds/enables something → to support someone else’s outcome*

Still, this framing encourages broader systems thinking. It highlights the interdependence of roles across organizations in a distributed system:

1. *As a* **data owner**  
   I get a report of currently **authorized data users** of my data, and a record of all applications, *so that*  
   I may fulfil my oversight responsibilities.

2. *As a* **data custodian** (access control),  
   I maintain a definitive, current record of which **data users** have been approved by **data owners** to access which datasets, *so that*  
   **data holders** may access a single, secure point of truth for authorization.

It facilitates gap analysis — surfacing missing interfaces, policies, or infrastructure:

1. *As a* **data steward**, I implement the **data owner’s** policies regarding appropriate use of data systems and **data users**’ data, *so that* systems and processes I am responsible for do comply with policy, minimizing the likelihood and impacts of misuse.

2. (where is the story that generates the ‘agreed policies’ consumed above?)

And it reframes operators, service providers and stewards as users, not just implementers. It can be empowering for a developer or administrator to consider themselves a user of the system they build or operate, and lead to more efficient design and process. 

[^1]:  An example of this in the European context is the [EGA dataset catalog](https://ega-archive.org/datasets/). An example of this in Australia in the broader (non-omics-specific) context is the [NCI Dataset Catalog](https://geonetwork.nci.org.au/geonetwork/srv/eng/catalog.search#/home).

[^2]:  Access to both the computational resources and the data in question may require authorization.

[^3]:  For example, by defining a role for each asset with an associated ‘read’ permission, and assigning the role to a group or user.

[^4]:  Something like the definition given here is common internationally in data governance and the Owner/Steward/Custodian taxonomy. But be aware that Australian Government bodies, e.g. the ABS and the NHMRC, often [don’t follow that](https://toolkit.data.gov.au/data-integration/roles-and-responsibilities/index.html) in their documentation, and use a single term ‘data custodian’ that broadly incorporates elements of data ownership and stewardship:  
| *Data custodians are agencies responsible for managing the use, disclosure and protection of source data*  
In my opinion the more granular separation of roles is useful in the biomedical research space.

[^5]:  Also known (e.g. in NSW Govt documents) as a Data sponsor.
