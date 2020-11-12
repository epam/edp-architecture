# EDP Components List

This page provides the list of EDP source code repositories that are used during the development process, as well as the corresponding descriptions of their purposes. 
For details, inspect the Table 1 below.

_Table 1. EDP Source Code Repositories._

|№| <nobr>Repository Name</nobr>  | Description  | 
|---|---|---|
|1| [All-EDP-Projects](https://gerrit-oc-green-edp-cicd.delivery.aws.main.edp.projects.epam.com/admin/repos/All-EDP-Projects) | It is an empty repository without code where RBAC policy is set, i.e. some resources, groups or users have access and all their rights are applied to other child repositories. |
|2| [All-Operators](https://gerrit-oc-green-edp-cicd.delivery.aws.main.edp.projects.epam.com/#/admin/projects/All-Operators) | It is an empty repository without code where RBAC policy is set, i.e. some resources, groups or users have access and all their rights are applied to other child repositories. | 
|3| [All-Projects](https://gerrit-oc-green-edp-cicd.delivery.aws.main.edp.projects.epam.com/#/admin/projects/All-Projects) | It is an empty repository without code where RBAC policy is set, i.e. some resources, groups or users have access and all their rights are applied to other child repositories. | 
|4| [All-Terraform](https://gerrit-oc-green-edp-cicd.delivery.aws.main.edp.projects.epam.com/#/admin/projects/All-Terraform) | It is an empty repository without code where RBAC policy is set, i.e. some resources, groups or users have access and all their rights are applied to other child repositories. |
|5| [All-Users](https://gerrit-oc-green-edp-cicd.delivery.aws.main.edp.projects.epam.com/#/admin/projects/All-Users)| It is an empty repository without code where RBAC policy is set, i.e. some resources, groups or users have access and all their rights are applied to other child repositories. |
|6| [edp-base](https://gerrit-oc-green-edp-cicd.delivery.aws.main.edp.projects.epam.com/admin/repos/edp-base) | It contains the Golang code with a base layer of EDP installation (cluster-wide tools like Keycloak, Monitoring tool, Logging tool, etc.). |
|7| [edp-install](https://gerrit-oc-green-edp-cicd.delivery.aws.main.edp.projects.epam.com/#/admin/projects/edp-install) | It contains the Helm Chart templates that describe the installation of the main configuration (e.g. database registration, user creation in a database, etc.), which cannot be subsumed to the corresponding operator or allotted to the repository.|
|8| [edp-install-wizard](https://gerrit-oc-green-edp-cicd.delivery.aws.main.edp.projects.epam.com/admin/repos/edp-install-wizard) | It contains the install wizard that is used for the EDP installation. | 
|9| [edp-admin-console](https://gerrit-oc-green-edp-cicd.delivery.aws.main.edp.projects.epam.com/admin/repos/edp-admin-console) | It contains the Golang code for the Admin Console application that is used for managing the EDP project. |
|10| [edp-library-pipelines](https://gerrit-oc-green-edp-cicd.delivery.aws.main.edp.projects.epam.com/#/admin/projects/edp-library-pipelines) | A Jenkins shared-library for the reference EDP pipelines. |
|11| [edp-library-stages](https://gerrit-oc-green-edp-cicd.delivery.aws.main.edp.projects.epam.com/#/admin/projects/edp-library-stages) | A Jenkins shared-library for the reference EDP stages. |
|12| [edp-jenkins](https://gerrit-oc-green-edp-cicd.delivery.aws.main.edp.projects.epam.com/#/admin/projects/edp-jenkins) | It contains the Dockerfile with a detailed description of how to build Jenkins including additional plugins and components installation. |
|13| [edp-gerrit](https://gerrit-oc-green-edp-cicd.delivery.aws.main.edp.projects.epam.com/admin/repos/edp-gerrit) | It contains the Dockerfile with a detailed description of how to build Gerrit including additional plugins and components installation. | 
|14| [edp-architecture](https://gerrit-oc-green-edp-cicd.delivery.aws.main.edp.projects.epam.com/admin/repos/edp-architecture) | It contains the general architecture of EPAM Delivery Platform. |
|15| [edp-autotests](https://gerrit-oc-green-edp-cicd.delivery.aws.main.edp.projects.epam.com/#/admin/projects/edp-autotests) | It contains all autotests necessary for the EDP verification. |
|16| [custom-pipelines](https://gerrit-oc-green-edp-cicd.delivery.aws.main.edp.projects.epam.com/#/admin/projects/custom-pipelines)| It contains the adapted EDP4EDP pipelines and stages that are used for EDP development. |
|17| [admin-console-operator](https://gerrit-oc-green-edp-cicd.delivery.aws.main.edp.projects.epam.com/admin/repos/admin-console-operator) | It deploys the Admin Console component on a cluster by using AdminConsole CR, which contains all necessary data. |
|18| [codebase-operator](https://gerrit-oc-green-edp-cicd.delivery.aws.main.edp.projects.epam.com/admin/repos/codebase-operator) | It prepares codebase repositories in order to use them in CI/CD process. |
|19| [cd-pipeline-operator](https://gerrit-oc-green-edp-cicd.delivery.aws.main.edp.projects.epam.com/admin/repos/cd-pipeline-operator) | It contains a set of controllers that are reconciled into EDP entities (e.g. Gerrit repository, Jenkins pipelines, etc.). |
|20| [reconciler](https://gerrit-oc-green-edp-cicd.delivery.aws.main.edp.projects.epam.com/admin/repos/reconciler) | It monitors all events, which happen with all CRs, and saves their representation into DB. |
|21| [gerrit-operator](https://gerrit-oc-green-edp-cicd.delivery.aws.main.edp.projects.epam.com/admin/repos/gerrit-operator) | It installs the Gerrit EDP Component in order to use it as GitProvider and store codebases code.|
|22| [jenkins-operator](https://gerrit-oc-green-edp-cicd.delivery.aws.main.edp.projects.epam.com/admin/repos/jenkins-operator) |It creates, deploys, and manages the EDP Jenkins instance on Kubernetes and OpenShift. In addition, the Jenkins instance is equipped with the necessary plugins. There is also the ability to customize the Jenkins instance as well as to check the changes during the application creation.|
|23| [keycloak-operator](https://gerrit-oc-green-edp-cicd.delivery.aws.main.edp.projects.epam.com/admin/repos/keycloak-operator) | It is responsible for establishing a connection to provided Keycloak Server, reconciling realms, and clients according to the created CRs. |
|24| [nexus-operator](https://gerrit-oc-green-edp-cicd.delivery.aws.main.edp.projects.epam.com/admin/repos/nexus-operator) | It installs the Nexus EDP Component on a cluster to store/manage artifacts of codebases. It also exposes configuration that allows Nexus to perform with other EDP components.  |
|25| [sonar-operator](https://gerrit-oc-green-edp-cicd.delivery.aws.main.edp.projects.epam.com/admin/repos/sonar-operator) | It installs the Sonar EDP Component on a cluster for continuous inspection of a codebase code quality. |
|26| [perf-operator](https://gerrit-oc-green-edp-cicd.delivery.aws.main.edp.projects.epam.com/admin/repos/perf-operator) | It is responsible for integration with the Project Performance Board (PERF board), maintenance, and creation of the data source in the delivery metrics. | 
|27| [edp-component-operator](https://gerrit-oc-green-edp-cicd.delivery.aws.main.edp.projects.epam.com/#/admin/projects/edp-component-operator) | It contains the API of EDP component that is necessary for the registry of the installed components. The Admin Console UI consists of several single components. | 
|28| [terraform-core](https://gerrit-oc-green-edp-cicd.delivery.aws.main.edp.projects.epam.com/admin/repos/terraform-core) | It is a core repository with Terraform code that is used for deploying infrastructure on OpenShift cluster in AWS. |
|29| [terraform-aws-vpc](https://gerrit-oc-green-edp-cicd.delivery.aws.main.edp.projects.epam.com/admin/repos/terraform-aws-vpc) | It contains Terraform code for VPC module as a part of Terraform AWS core that is used for provisioning and configuration VPC on a top of AWS. |
|30| [terraform-aws-openshift](https://gerrit-oc-green-edp-cicd.delivery.aws.main.edp.projects.epam.com/admin/repos/terraform-aws-openshift) | It contains Terraform code for OpenShift module as a part of Terraform AWS core that is used for provisioning and configuration EC2 infrastructure on top of AWS. |
|31| [terraform-aws-init](https://gerrit-oc-green-edp-cicd.delivery.aws.main.edp.projects.epam.com/admin/repos/terraform-aws-init) | It contains a Terraform code for the Init module as a part of Terraform AWS core that is used for the initialization of the backend for the Terraform state file. |
|32| [terraform-aws-dns](https://gerrit-oc-green-edp-cicd.delivery.aws.main.edp.projects.epam.com/admin/repos/terraform-azure-dns) | It contains a Terraform code for the DNS module as a part of Terraform AWS core that is used for provisioning and configuration of the Route53 service in AWS. |
|33| [terraform-aws-bastion](https://gerrit-oc-green-edp-cicd.delivery.aws.main.edp.projects.epam.com/admin/repos/terraform-aws-bastion) | It contains a Terraform code for the Bastion module as a part of Terraform AWS core that is used for provisioning Bastion host for external access to infrastructure in AWS. |


### Related Articles

- [EPAM Delivery Platform Overview](https://github.com/epmd-edp/edp-install/tree/master#epam-delivery-platform-rocket)
- [EDP Architecture](https://github.com/epmd-edp/edp-architecture#edp-architecture) 

