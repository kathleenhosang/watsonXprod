# watsonX Production Deployments
WatsonX On Premise Production Checklist

## Architecture Overview

<img width="785" alt="Screenshot 2023-05-25 at 2 28 47 PM" src="https://github.com/kathleenhosang/sno/assets/40863347/ff048dc6-41bc-466c-8271-472409d54bcf">


## WatsonX.ai Checklist
Requirement | Details | Documentation |
--------|--------|--------|
Model Selection | List models that the client requires, this determines sizing | [Adding Foundational Models to WatsonX](https://www.ibm.com/docs/en/cloud-paks/cp-data/4.8.x?topic=setup-adding-foundation-models) |
Storage Selection | *ODF, Fusion, Px, AWS <br /> *NFS not recommended because snapshots are not supported for BRDR <br /> *Azure native storage not supported by foundational services WA/ WD supports ODF, IBM storage, or Px | [Storage Architecture](https://www.ibm.com/docs/en/cloud-paks/cp-data/4.8.x?topic=architecture-storage) <br /> [Storage Requirements](https://www.ibm.com/docs/en/cloud-paks/cp-data/4.8.x?topic=requirements-storage) |
Sizing | *Assume HA is required <br /> *Multi pod per service should be selected in sales configurator | [Sales Configurator](https://app.ibmsalesconfigurator.com/#/)
GPU | *GPU SKU selection <br /> *Attaching GPU nodes to cluster for optimal performance and cost | [Adding GPU to Cluster](https://www.ibm.com/docs/en/mas-cd/continuous-delivery?topic=inspection-enabling-gpu-passthrough)
Client Internal Reviews | Understand client’s internal review process to put WatsonX in production (any additional security reviews, architectural reviews, business process reviews, etc)
Installation Approach | * OpenShift (IPI v UPI, platform, storage, networking requirements, security requirements, etc) <br /> *Cloud Pak <br /> *WatsonX |
Day 2 Operations | *Logging and Monitoring <br /> *LDAP <br /> *Certificate Management |
BR/ DR | *Data replication <br /> *Data recovery <br /> *Back up and restore <br /> *Understand services limitations <br /> *If this is a requirement, cpd OADP based BRDR tooling should be used as a best practice, with IBM Fusion or ODF |
Security | *Security Scans <br /> *Data Isolation <br /> *Application Security | |

## WatsonX.data Checklist
Requirement | Details | Documentation |
--------|--------|--------|
Coming soon 

## WatsonX.gov Checklist
Requirement | Details | Documentation |
--------|--------|--------|
Coming Soon
