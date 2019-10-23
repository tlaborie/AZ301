# AZ301
## AZ-301 Study Guide and Materials for Exam

#### Skills measured:

+ [Determine workload requirements](#determine-workload-requirements-10-15)
+ [Design for identity and security](#design-for-identity-and-security-20-25)
+ [Design a data platform solution](#design-a-data-platform-solution-15-20)
+ [Design a business continuity strategy](#design-a-business-continuity-strategy-15-20)
+ [Design for deployment, migration, and integration](#design-for-deployment-migration-and-integration-10-15)
+ [Design an infrastructure strategy](#design-an-infrastructure-strategy-15-20)

#### External Resources

 + [Pluralsight - Learning Path - Microsoft Azure Architect Design (AZ-301)](https://www.pluralsight.com/paths/microsoft-azure-architect-design-az-301)

## Determine workload requirements (10-15%)

#### Gather Information and Requirements

+ identify [compliance requirements](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/ready/azure-readiness-guide/govern-org-compliance?tabs=AzureBlueprints), [identity](https://docs.microsoft.com/en-us/azure/security/fundamentals/identity-management-best-practices) and [access management infrastructure](https://docs.microsoft.com/en-us/azure/security/fundamentals/identity-management-best-practices), and
[service-oriented architectures](https://docs.microsoft.com/en-us/dotnet/architecture/microservices/architect-microservice-container-applications/service-oriented-architecture) (e.g., [integration patterns](https://docs.microsoft.com/en-us/azure/architecture/patterns/), [service design](https://docs.microsoft.com/en-us/azure/architecture/), [service
discoverability](https://docs.microsoft.com/en-us/dotnet/architecture/microservices/architect-microservice-container-applications/microservices-addressability-service-registry)
+ identify accessibility (e.g. [Web Content Accessibility Guidelines](https://www.microsoft.com/en-us/trustcenter/compliance/compliance-offerings/wcag)), availability (e.g. [Service Level Agreement](https://azure.microsoft.com/en-us/support/legal/sla/summary/)), capacity planning and scalability, deploy-ability (e.g., repositories,
failback, slot-based deployment), configurability, [governance](https://docs.microsoft.com/en-us/azure/governance/azure-management), maintainability (e.g.
logging, debugging, troubleshooting, recovery, training), security (e.g. authentication,
authorization, attacks), and sizing (e.g. support costs, optimization) requirements
+ [recommend changes during project execution (ongoing)]()
+ [evaluate products and services to align with solution]()
+ [create testing scenarios](https://azure.microsoft.com/en-us/solutions/dev-test/#references/)

##### External Resources: 
+ [Pluralsight - Gathering Information About Existing Enterprise Architecture in Microsoft Azure](https://www.pluralsight.com/courses/microsoft-azure-enterprise-architecture-information-gathering)
+ [Pluralsight - Gathering Non-functional Requirements for Microsoft Azure](https://app.pluralsight.com/library/courses/microsoft-azure-non-functional-requirements-gathering/table-of-contents)
+ [Pluralsight - Determining Feasibility and Refining Requirements for Microsoft Azure](https://app.pluralsight.com/library/courses/microsoft-azure-feasibility-determining-requirements-refining)

#### Optimize Consumption Strategy
+ [optimize app service, compute, identity, network, and storage costs](https://docs.microsoft.com/en-us/azure/cost-management/)

##### External Resources
+ [Pluralsight - Estimating One-time and Recurring Costs for Microsoft Azure](https://app.pluralsight.com/library/courses/microsoft-azure-one-time-costs-estimating-recurring)
+ [Pluralsight- Optimizing Consumption Strategy in Microsoft Azure](https://www.pluralsight.com/courses/microsoft-azure-consumption-strategy-optimizing)

#### Design an Auditing and Monitoring Strategy

+ [define logical groupings (tags) for resources to be monitored](https://docs.microsoft.com/en-us/azure/azure-resource-manager/resource-group-using-tags)
+ [determine levels and storage locations for logs](https://docs.microsoft.com/en-us/azure/azure-monitor/platform/resource-logs-overview)
+ [plan for integration with monitoring tools](https://azure.microsoft.com/en-us/blog/use-azure-monitor-to-integrate-with-siem-tools/)
+ [recommend appropriate monitoring tool(s) for a solution](https://docs.microsoft.com/en-us/azure/azure-monitor/overview) ([additional tools]https://docs.microsoft.com/en-us/azure/azure-monitor/insights/solutions)
+ [specify mechanism for event routing and escalation](https://docs.microsoft.com/en-us/azure/event-grid/overview)
+ [design auditing for compliance requirements](https://docs.microsoft.com/en-us/azure/security/fundamentals/log-audit)
+ [design auditing policies and traceability requirements](https://docs.microsoft.com/en-us/azure/security/fundamentals/log-audit)

##### External Resources

+ [Pluralsight - Designing a Monitoring Strategy for a Solution in Microsoft Azure](https://app.pluralsight.com/library/courses/microsoft-azure-monitoring-strategy-solution-designing)
+ [Pluralsight - Design Auditing for Microsoft Azure](https://app.pluralsight.com/library/courses/microsoft-azure-auditing-design)

## Design for identity and security (20-25%)

#### Design Identity Management
+ [choose an identity management approach](https://docs.microsoft.com/en-us/azure/security/fundamentals/identity-management-overview)
+ [design an identity delegation strategy, identity repository (including directory,
application, systems, etc.](https://docs.microsoft.com/en-us/windows-server/identity/ad-fs/design/when-to-use-identity-delegation)
+ [design self-service identity management and user and persona provisioning](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/methods-for-assigning-users-and-groups)
+ [define personas and roles](https://docs.microsoft.com/en-us/azure/active-directory/users-groups-roles/)
+ [recommend appropriate access control strategy (e.g., attribute-based, discretionary
access, history-based, identity-based, mandatory, organization-based, role-based, rulebased, responsibility-based)](https://docs.microsoft.com/en-us/azure/security/fundamentals/identity-management-best-practices)

##### External Resources
+ [Pluralsight - Design Identity Management in Microsoft Azure](https://app.pluralsight.com/library/courses/microsoft-azure-identity-management-design)

#### Design Authentication
+ [choose an authentication approach](https://docs.microsoft.com/en-us/azure/security/fundamentals/choose-ad-authn)
+ [design a single-sign on approach](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/what-is-single-sign-on)
+ [design for IPSec, logon, multi-factor, network access, and remote authentication](https://docs.microsoft.com/en-us/azure/active-directory/develop/authentication-scenarios)

##### External Resources
+ [Pluralsight - Design Authentication for Microsoft Azure](https://www.pluralsight.com/courses/microsoft-azure-authentication-design)

#### Design Authorization
+ [choose an authorization approach]()
+ [define access permissions and privileges]()
+ design secure delegated access (e.g., oAuth, OpenID, etc.)
  + (https://docs.microsoft.com/en-us/azure/active-directory/develop/developer-glossary#permissions)
  + (https://docs.microsoft.com/en-us/azure/active-directory/develop/v1-protocols-oauth-code)
  + (https://docs.microsoft.com/en-us/azure/active-directory/develop/v1-protocols-oauth-code)
+ [recommend when and how to use API Keys](https://docs.microsoft.com/en-us/azure/api-management/api-management-howto-protect-backend-with-aad)

##### External Resources
+ [Pluralsight - Design Authorization for Microsoft Azure ](https://app.pluralsight.com/library/courses/microsoft-azure-authorization-design)

#### Design for Risk Prevention for Identity
+ design a risk assessment strategy (e.g., [access reviews](https://docs.microsoft.com/en-us/azure/active-directory/governance/access-reviews-overview), [RBAC policies, physical access](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-risk-events))
+ evaluate agreements involving services or products from vendors and contractors
+ update solution design to address and mitigate changes to existing security policies,
standards, guidelines and procedures

##### External Resources
+ [Pluralsight - Design for Risk Prevention in Microsoft Azure](https://app.pluralsight.com/library/courses/microsoft-azure-risk-prevention-design)

#### Design a Monitoring Strategy for Identity and Security
+ [design for alert notifications](https://docs.microsoft.com/en-us/azure/azure-monitor/platform/alerts-overview)
+ [design an alert and metrics strategy](https://docs.microsoft.com/en-us/azure/azure-monitor/platform/alerts-metric)
+ [recommend authentication monitors](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/overview-monitoring)

 ##### External Resources 
 +[Pluralsight - Design a Monitoring Strategy for Identity and Security in Microsoft Azure](https://app.pluralsight.com/library/courses/microsoft-azure-monitoring-strategy-identity-security-design)

## Design a data platform solution (15-20%)

#### Design a Data Management Strategy
+ [choose between managed and unmanaged data store]()
+ [choose between relational and non-relational databases](https://docs.microsoft.com/en-us/azure/architecture/guide/technology-choices/data-store-overview)
+ [design data auditing and caching strategies](https://docs.microsoft.com/en-us/azure/architecture/best-practices/caching)
+ [identify data attributes (e.g., relevancy, structure, frequency, size, durability, etc.)]()
+ [recommend Database Transaction Unit (DTU) sizing](https://docs.microsoft.com/en-us/azure/sql-database/sql-database-service-tiers-dtu)
+ [design a data retention policy](https://docs.microsoft.com/en-us/azure/sql-database/sql-database-long-term-retention)
+ [design for data availability, consistency, and durability]()
+ [design a data warehouse strategy](https://docs.microsoft.com/en-us/azure/sql-data-warehouse/sql-data-warehouse-overview-what-is)

##### External Resources
+ [Pluralsight - Design a Data Management Strategy for Microsoft Azure](https://app.pluralsight.com/library/courses/microsoft-azure-data-management-strategy-design)
+ [Pluralsight - Plan for Data Warehousing with Microsoft Azure](https://app.pluralsight.com/library/courses/microsoft-azure-data-warehousing-plan)

#### Design a Data Protection Strategy
+ [recommend geographic data storage](https://docs.microsoft.com/en-us/azure/storage/common/storage-redundancy)
+ [design an encryption strategy for data at rest, for data in transmission, and for data in
use](https://docs.microsoft.com/en-us/azure/security/fundamentals/encryption-overview)
+ [design a scalability strategy for data](https://docs.microsoft.com/en-us/azure/architecture/checklist/scalability)
+ [design secure access to data](https://docs.microsoft.com/en-us/azure/security/fundamentals/data-encryption-best-practices)
+ [design a data loss prevention (DLP) policy](https://docs.microsoft.com/en-us/flow/prevent-data-loss)

##### External Resources
+ [Pluralsight - Design a Data Protection Strategy with Microsoft Azure](https://app.pluralsight.com/library/courses/microsoft-azure-data-protection-strategy-design)

#### Design and Document Data Flows
+ [identify data flow requirements](https://docs.microsoft.com/en-us/azure/data-factory/concepts-data-flow-overview)
+ [create a data flow diagram](https://docs.microsoft.com/en-us/azure/data-factory/data-flow-create)
+ [design a data flow to meet business requirements](https://docs.microsoft.com/en-us/azure/data-factory/concepts-data-flow-schema-drift)
+ [design a data import and export strategy](https://docs.microsoft.com/en-us/azure/storage/common/storage-import-export-service)

##### External Resources
+ [Pluralsight - Design and Document Data Flows with Microsoft Azure](https://app.pluralsight.com/library/courses/microsoft-azure-data-flows-document-design)

#### Design a Monitoring Strategy for the Data Platform
+ [design for alert notifications](https://docs.microsoft.com/en-us/azure/azure-monitor/platform/alerts-overview)
+ [design an alert and metrics strategy](https://docs.microsoft.com/en-us/azure/azure-monitor/platform/data-sources#options-for-data-consumption)


## Design a business continuity strategy (15-20%)

#### Design a Site Recovery Strategy
+ [design a recovery solution](https://docs.microsoft.com/en-us/azure/site-recovery/site-recovery-overview)
+ [design a site recovery replication policy](https://docs.microsoft.com/en-us/azure/site-recovery/vmware-azure-set-up-replication)
+ [design for site recovery capacity and for storage replication](https://docs.microsoft.com/en-us/azure/site-recovery/site-recovery-plan-capacity-vmware)
+ [design site failover and failback (planned/unplanned)](https://docs.microsoft.com/en-us/azure/site-recovery/site-recovery-failover)
+ [design the site recovery network](https://docs.microsoft.com/en-us/azure/site-recovery/azure-to-azure-about-networking)
+ [recommend recovery objectives (e.g., Azure, on-prem, hybrid, Recovery Time Objective
(RTO), Recovery Level Objective (RLO), Recovery Point Objective (RPO))](https://docs.microsoft.com/en-us/azure/site-recovery/site-recovery-overview)
+ [identify resources that require site recovery](https://docs.microsoft.com/en-us/azure/site-recovery/site-recovery-workload)
+ [identify supported and unsupported workloads](https://docs.microsoft.com/en-us/azure/site-recovery/vmware-physical-azure-support-matrix)
+ [recommend a geographical distribution strategy]()

##### External Resources
+ [Designing a Site Recovery Strategy on Microsoft Azure](https://www.pluralsight.com/courses/microsoft-azure-site-recovery-strategy-designing)

#### Design for High Availability
+ design for [application redundancy](https://docs.microsoft.com/en-us/azure/architecture/reliability/), [autoscaling](https://docs.microsoft.com/en-us/azure/architecture/best-practices/auto-scaling), [data center and fault domain
redundancy, and network redundancy](https://docs.microsoft.com/en-us/azure/architecture/reliability/)
+ [identify resources that require high availability](https://docs.microsoft.com/en-us/azure/architecture/checklist/resiliency-per-service)
+ [identify storage types for high availability](https://docs.microsoft.com/en-us/azure/storage/blobs/storage-blob-storage-tiers)

##### External Resources
+ [Pluralsight - Designing for High Availability on Microsoft Azure](https://app.pluralsight.com/library/courses/microsoft-azure-high-availability-designing)

#### Design a Data Archiving Strategy
+ [recommend storage types and methodology for data archiving]()
+ [identify requirements for data archiving and business compliance requirements for data
archiving]()
+ [identify SLA(s) for data archiving]()

## Design for deployment, migration, and integration (10-15%)

#### Design Deployments
+ [design a compute, container, data platform, messaging solution, storage, and web app
and service deployment strategy]()

#### Design Migrations
+ [recommend a migration strategy]()
+ [design data import/export strategies during migration]()
+ [determine the appropriate application migration, data transfer, and network connectivity
method]()
+ [determine migration scope, including redundant, related, trivial, and outdated data]()
+ [determine application and data compatibility]()

#### Design an API Integration Strategy
+ [design an API gateway strategy]()
+ [determine policies for internal and external consumption of APIs]()
+ [recommend a hosting structure for API management]()

## Design an infrastructure strategy (15-20%)

#### Design a Storage Strategy
+ [design a storage provisioning strategy]()
+ [design storage access strategy]()
+ [identify storage requirements]()
+ [recommend a storage solution and storage management tools]()

#### Design a Compute Strategy
+ [design compute provisioning and secure compute strategies]()
+ [determine appropriate compute technologies (e.g., virtual machines, functions, service
fabric, container instances, etc.)]()
+ [design an Azure HPC environment]()
+ [identify compute requirements]()
+ [recommend management tools for compute]()

#### Design a Networking Strategy
+ [design network provisioning and network security strategies]()
+ [determine appropriate network connectivity technologies]()
+ [identify networking requirements]()
+ [recommend network management tools]()

#### Design a Monitoring Strategy for Infrastructure
+ [design for alert notifications]()
+ [design an alert and metrics strategy]()

