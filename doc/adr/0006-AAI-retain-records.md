# 6. Aai retain records

Date: 2025-09-24

## Status

Accepted

## Context

University of Melbourne are the host organization of Australian BioCommons and as such their institutional policies around record retention apply to data collected for the purposes of BioCommons operating an AAI solution. In particular — as part of the privacy impact assessment associated with BioCommons' CILogon subscription — the University RDA document section 15.2.1: Information security was determined to hold:
> TECHNOLOGY & APPLICATIONS | Information Security
> 15.2.1: Information security
> Records relating to the security of information systems.
> For example, records associated with establishing and assigning security levels and caveats within records management systems.
> Required action: Temporary - Destroy 7 years after system becomes defunct or is superseded.
In the context of CILogon we interpret this as records (e.g. logs) relating to user registration and group assignment actions.

## Decision

Logs archived after AAI system operation ceases will be securely archived in an AWS bucket with a lifecycle policy set to auto-delete objects after 2555 days.

## Consequences

By doing this we are compliant with University policy. A risk is that institutional knowledge may not persist in the long gap between last operation and destroy date. This can be mitigated by suitable naming of the bucket and an in-situ README file providing context.
