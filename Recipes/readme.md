# Integration Recipes
\| Browsing by Topic \| [Browse by Author](author.md) \| [Browse by Artefact Type](for/readme.md) \| [Request a Recipe](https://github.com/SAP-samples/cloud-integration-flow/issues/new?assignees=&labels=Recipe%20Request&template=recipe-request.md&title=How+to++) \| [Report a broken link](https://github.com/SAP-samples/cloud-integration-flow/issues/new?assignees=&labels=documentation&template=bug_report.md&title=Broken%20Link) \| [Contribute](https://github.com/SAP-samples/cloud-integration-flow/wiki/Things-to-do-on-this-repo#contribute)\|

## Topics
* [Amazon](#amazon-web-services)
* [CICD](#cicd)
* [Database Connectivity](#amazon-developer-connectivity)
* [How to Guides](#how-to-guide)
* [Integration Adapters](#integration-adapters)
* [Integration Patterns](#integration-patterns)
* [Mappings](#mappings)
* [Partner Directory](#partner-directory)
* [Qualtrics](#qualtrics)
* [SAP Ariba or SAP Business Network](#sap-ariba)
* [SAP Concur](#sap-concur)
* [SAP Customer Experience](#sap-customer-experience)
* [SAP Document Compliance](#sap-document-compliance)
* [SAP ERP](#sap-erp)
* [SAP S/4HANA](#sap-s4hana)
* [SAP S/4HANA Cloud](#sap-s4hana-cloud)
* [SAP SuccessFactors Employee Central](#sap-successfactors-employee-central)
* [Third-Party Integration](#third-party-integration)
* [Security](#security)


***

### Amazon
Recipe|Description|Author
---|---|---
[Amazon Seller Marketplace Integration with Third Party](for/amazonsellermarketplaceintegrationwiththirdparty)|File based integration for sending Sales Transaction data from Amazon Seller Marketplace to Third Party (SAP Vistex template)  | [SAP API Business Hub](author.md#sap-api-business-hub)
[Connect to Amazon DynamoDB](for/ConnectToAWSDynmoDB)|SAP CPI needs to make a rest call to DynamoDB endpoint.|[Sunny Kapoor](author.md#sunny-kapoor)|
[Generate AWS4-HMAC-SHA256 Signature](for/GenerateAWS4_HMAC_SHA256)| A reusable recipe to generate an AWS specific AWS4-HMAC-SHA256 signature and pass it as a HTTP Authorization header.|[Sunny Kapoor](author.md#sunny-kapoor)|

***

### CICD

Recipe|Description|Author
---|---|---
[Deploy Integration Artefact and Get Endpoint](for/CICD-DeployIntegrationArtefactGetEndpoint)|Deploy an existing integration flow on Cloud Integration runtime. Optionally you can also get the endpoint of the integration flow.| [Axel Albrecht](author.md#axel-albrecht) |
[Deploy Run Once Integration Artefact and Check MPL](for/CICD-DeployRunOnceIntegrationArtefactAndCheckMpl)|Deploy an integration flow, check its deployment status and the message processing log status of the message execution that gets automatically triggered after the deployment due to a scheduler configuration or the consumption of files from a (S)FTP server or messages from a JMS queue.| [Axel Albrecht](author.md#axel-albrecht) |
[Deploy Run Once Integration Artefact and Check MPL and Store If Success](for/CICD-DeployRunOnceIntegrationArtefactAndCheckMplAndStoreIfSuccess)|Deploy an integration flow, check its deployment status and the MPL (message processing log) status. In case of a successful message processing the job then downloads the integration flow artefact from the Cloud Integration tenant and commits it to the source code repository.| [Mayur Mohan Belur](author.md#mayur-mohan-belur) |
[Get Latest Message Processing Log](for/CICD-GetLatestMessageProcessingLog)|Get the status of the last message execution of the configured integration artefact. In case the message execution failed, the job also provides the error information.| [Axel Albrecht](author.md#axel-albrecht) |
[Get Specific Message Processing Log](for/CICD-GetSpecificMessageProcessingLog)|Get the message procesing log status of either a specific message exchange ID or of the last run of a specific integration artefact. In case the message execution failed, the job also provides the error information.| [Axel Albrecht](author.md#axel-albrecht) |
[Store All API Providers](for/CICD-StoreAllAPIProviders)|Download all API Providers from the API Portal and store it in your source code repository like Git.|[Mahesh Srikrishnan](author.md#mahesh-srikrishnan)|
[Store Integration Artefact](for/CICD-StoreIntegrationArtefact)|Download a specific integration artefact from the Cloud Integration tenant and store it in your source code repository like Git.| [Axel Albrecht](author.md#axel-albrecht) |
[Store Integration Artefact on New Version](for/CICD-StoreIntegrationArtefactOnNewVersion)|Check the Cloud Integration tenant for a new version of your integration artefact and if a new version exists, it downloads and stores it in a source code repository like Git.| [Axel Albrecht](author.md#axel-albrecht) |
[Store Single API Provider](for/CICD-StoreSingleAPIProvider)|Download a specific API Provider from the API Portal and store it in your source code repository like Git.|[Mahesh Srikrishnan](author.md#mahesh-srikrishnan)|
[Store Single API Proxy](for/CICD-StoreSingleAPIProxy)|Download a specific API Proxy from the API Portal and store it in your source code repository like Git.|[Mahesh Srikrishnan](author.md#mahesh-srikrishnan)|
[Store Single Key Value Map](for/CICD-StoreSingleKeyValueMap)|Download a specific Key Value Map from the API Portal and store it in your source code repository like Git.|[Mahesh Srikrishnan](author.md#mahesh-srikrishnan)|
[Undeploy Integration Artefact](for/CICD-UndeployIntegrationArtefact)|Undeploy a specific integration artefact from the Cloud Integration tenant.| [Axel Albrecht](author.md#axel-albrecht) |
[Update Integration Configuration Parameter](for/CICD-UpdateIntegrationConfigurationParameter)|Configure the value of an externalized parameter of a specific integration artefact in the Cloud Integration tenant.| [Axel Albrecht](author.md#axel-albrecht) |
[Update Integration Resources on Git Commit](for/CICD-UpdateIntegrationResourcesOnGitCommit)|Develop and manage your integration resources like scripts and XSLT mappings using external IDEs and SCM tools like Git.|[Sunny Kapoor](author.md#sunny-kapoor)|
[Upload Integration Artefact](for/CICD-UploadIntegrationArtefact)|Checkout the latest version of the configured integration flow artefact from your source code repository and either update or create the artefact on the Cloud Integration tenant.| [Mayur Mohan Belur](author.md#mayur-mohan-belur) |
[Upload Single API Provider](for/CICD-UploadSingleAPIProvider)|Checkout the configured API Provider from the source code repository and either update or create the artefact on the API Portal tenant.|[Sunny Kapoor](author.md#sunny-kapoor)|
[Upload Single API Proxy](for/CICD-UploadSingleAPIProxy)|Checkout the configured API Proxy from the source code repository and either update or create the artefact on the API Portal tenant.|[Sunny Kapoor](author.md#sunny-kapoor)|
[Upload Single Key Value Map](for/CICD-UploadSingleKeyValueMap)|Checkout the configured Key Value Map from the source code repository and either update or create the artefact on the API Portal tenant.|[Sunny Kapoor](author.md#sunny-kapoor)|

***

### Database Connectivity
Recipe|Description|Author
---|---|---
[Connect to Amazon DynamoDB](for/ConnectToAWSDynmoDB)|SAP CPI needs to make a rest call to DynamoDB endpoint.|[Sunny Kapoor](author.md#sunny-kapoor)|

***

### How to Guides
Recipe|Description|Author
---|---|---
[Simulate Response from Datastore Select Operation and Write Variable](for/SimulateResponseFromWriteVariableAndDataStores)|Test a still under development integration flow with dummy data without the need for deployment. This recipe simulate reading of Write Variable in Content Modifier and the Datastore Select operation.|[Abhinav Verma](author.md#abhinav-verma)|

***

### Integration Adapters
Recipe|Description|Author
---|---|---
[Build custom Azure Blob Storage integration adapter](for/azure-integration-adapter/readme.md)| Azure Blob Storage is a massively scalable and secure object storage for cloud-native workloads, archives, data lakes, high-performance computing and machine learning. The camel-Azure Blob Storage component stores and retrieves blobs from [Azure Storage Blob Service](https://azure.microsoft.com/services/storage/blobs/) using Azure APIs v12. This integration adapter enables an integration flow to connect to Azure Blob Storage collection.|[Mayur Mohan Belur](author.md#mayur-mohan-belur) |
[Build custom MongoDB integration adapter](for/mongodb-integration-adapter/readme.md)|MongoDB is a very popular NoSQL solution and the camel-mongodb component integrates Camel with MongoDB allowing you to interact with MongoDB collections both as a producer (performing operations on the collection) and as a consumer (consuming documents from a MongoDB collection). This integration adapter enables an integration flow to connect to MongoDb collection.| [Mayur Mohan Belur](author.md#mayur-mohan-belur) |
[Build custom Rabbit MQ integration adapter](for/redis-integration-adapter/readme.md)|The rabbitmq: component allows you produce and consume messages from RabbitMQ instances. Using the RabbitMQ AMQP client, this component offers a pure RabbitMQ approach over the generic AMQP component. This integration adapter enables an integration flow to persist or read messages in a RabbitMQ queue. | [Mayur Mohan Belur](author.md#mayur-mohan-belur) |
[Build custom Redis integration adapter](for/redis-integration-adapter/readme.md)|Redis is advanced key-value store where keys can contain strings, hashes, lists, sets and sorted sets. In addition it provides pub/sub functionality for inter-app communications. This integration adapter allows an integration flow to access Redis.| [Mayur Mohan Belur](author.md#mayur-mohan-belur)|

***
### Integration Patterns
Recipe|Description|Author
---|---|---
[Command Message](for/EIP-MessageConstruction-CommandMessage/readme.md)| This recipe lets you try out Command Message pattern for SOAP, OData and a BAPI.| [Bhalchandra Wadekar](author.md#bhalchandra-wadekar)|
[Correlation Identifier](for/EIP-MessageConstruction-CorrelationIdentifier/readme.md)| When sending the request, the sender adds a unique key to request. The receiver processes the request and puts the unique key as the Correlation Identifier in the reply message. Thus when a reply is received independent of the request, the sender knows the request corresponding the received reply based on the Correlation Identifier. |  [Bhalchandra Wadekar](author.md#bhalchandra-wadekar)|
[Document Message](for/EIP-MessageConstruction-DocumentMessage/readme.md)|This recipe lets you send a Email using the Document Message pattern. |[Bhalchandra Wadekar](author.md#bhalchandra-wadekar)|
[Event Message](for/EIP-MessageConstruction-EventMessage/readme.md)|This recipe lets you send a product update using the Event Message pattern.|[Bhalchandra Wadekar](author.md#bhalchandra-wadekar)|
[Request Reply](for/EIP-MessageConstruction-Request-Reply/readme.md)|This recipe retrieves a list of products using the Request-Reply pattern.|[Bhalchandra Wadekar](author.md#bhalchandra-wadekar)|
[Return Address](for/EIP-MessageConstruction-ReturnAddress/readme.md) | This recipe lets you try out Return Address pattern.| [Bhalchandra Wadekar](author.md#bhalchandra-wadekar)|

***

### Mappings
Recipe|Description|Author
---|---|---
[Accessing Value Mappings from Groovy script](for/AccessValueMappingsDynamicallyScript)|Use ```ITApiFactory.getApi()``` to get ```ValueMappingAPI``` class that can be used to retrieve the mappings.|[Sharad Dixit](author.md#sharad-dixit)|
[Convert JSON to XML using XSLT Mappings](for/ConvertJsonToXMLusingXSLT30)|This recipe converts and incoming file from JSON format to XML format.|[Kamlesh Zanje](author.md#kamlesh-zanje)|
[Invoke Java functions from XSLT Mapping](for/InvokeJavaFunctionsFromXSLT30)|Writing reflexive extension functions in Java to be invoked from XSLT.|[Kamlesh Zanje](author.md#kamlesh-zanje)|
[Use Map data structures in XSLT Mapping](for/ConstructMapDataStructsUsingXSLT30)|Utilize [Map](https://www.w3.org/TR/xslt-30/#map) data structures in XSLT Mappings flow step.|[Kamlesh Zanje](author.md#kamlesh-zanje) |

***

### Partner Directory
Recipe|Description|Author
---|---|---
[Accessing Partner Directory entries from within a Groovy script](for/Accessing-Partner-Directory-entries-from-within-a-script)|The String and Binary parameters from the Partner Directory can be accessed using a script with the help of getParameter API of the PartnerDirectoryService class. | [Amrita Laxmi](author.md#amrita-laxmi) |

***

### [Qualtrics](#qualtrics)

Recipe|Description|Author
---|---|---
[Qualtrics Transaction-Based Survey Integration with SAP Marketing Cloud](for/qualtricsextendedintegrationwithsapmarketingcloud)| Load data (customers and transactions with transcation based interaction in Marketing cloud) from SAP Marketing Cloud system to SAP Qualtrics. |[SAP API Business Hub](author.md#sap-api-business-hub)

***

### SAP Ariba
Recipe|Description|Author
---|---|---
[ SAP Ariba Integration with Third-Party for Analytical Reporting](for/saparibaanalyticalreportingintegrationwiththirdparty)| Consumption of Ariba APIs (Job Submission API and Job Results API) for Analytical Reporting ( Standard/Custom Templates) with CSV Output for integrating with Third Party  |[SAP API Business Hub](author.md#sap-api-business-hub)
[SAP Ariba Integration with Third-Party for Vendor And Questionnaires](for/saparibaintegrationwiththirdpartyforvendorandquestionnaires)| Ariba APIs for Vendor and Questionnaires with CSV Output for integrating with Third Party| ionnaires)| |[SAP API Business Hub](author.md#sap-api-business-hub)
[SAP Business Network Integration with Non-SAP ERP](for/sapbusinessnetworkintegrationwithnonsaperp)| Baseline template to support the Purchase Order, Invoice and other transactional documents with the SAP Business Network|[SAP API Business Hub](author.md#sap-api-business-hub)

***

### SAP Concur
Recipe|Description|Author
---|---|---


***

### SAP Customer Experience
Recipe|Description|Author
---|---|---
[Qualtrics Transaction-Based Survey Integration with SAP Marketing Cloud](for/qualtricsextendedintegrationwithsapmarketingcloud)| Load data (customers and transactions with transcation based interaction in Marketing cloud) from SAP Marketing Cloud system to SAP Qualtrics. |[SAP API Business Hub](author.md#sap-api-business-hub)


***

### SAP Document Compliance

Recipe|Description|Author
---|---|---
[SAP Document Compliance with Third Party - eDocuments](for/saps4hanaintegrationwiththirdpartyedocuments)| Exchange electronic invoices with the tax authorities for Chile, Colombia and Mexico, available for SAP S/4HANA, and SAP ERP (available as of SAP ERP 6.0 EHP5)|[SAP API Business Hub](author.md#sap-api-business-hub)


***

### SAP ERP
Recipe|Description|Author
---|---|---
[SAP Document Compliance with Third Party - eDocuments](for/saps4hanaintegrationwiththirdpartyedocuments)| Exchange electronic invoices with the tax authorities for Chile, Colombia and Mexico, available for SAP S/4HANA, and SAP ERP (available as of SAP ERP 6.0 EHP5)|[SAP API Business Hub](author.md#sap-api-business-hub)
[SAP SuccessFactors Employee Central Payroll Integration with SAP S_4HANA or SAP ERP](for/sapsuccessfactorsemployeecentralpayrollintegrationwithsaps4hanaorsaperp)| Replication of Payroll posting data from SAP SuccessFactors Employee Central to SAP ERP or SAP S/4HANA. This data includes Cost Center/GL accounts/Expenses.|[SAP API Business Hub](author.md#sap-api-business-hub)


***

### SAP S4HANA
Recipe|Description|Author
---|---|---
[SAP Document Compliance with Third Party - eDocuments](for/saps4hanaintegrationwiththirdpartyedocuments)| Exchange electronic invoices with the tax authorities for Chile, Colombia and Mexico, available for SAP S/4HANA, and SAP ERP (available as of SAP ERP 6.0 EHP5)|[SAP API Business Hub](author.md#sap-api-business-hub)
[SAP SuccessFactors Employee Central Payroll Integration with SAP S_4HANA or SAP ERP](for/sapsuccessfactorsemployeecentralpayrollintegrationwithsaps4hanaorsaperp)| Replication of Payroll posting data from SAP SuccessFactors Employee Central to SAP ERP or SAP S/4HANA. This data includes Cost Center/GL accounts/Expenses.|[SAP API Business Hub](author.md#sap-api-business-hub)


***

### SAP S4HANA Cloud
Recipe|Description|Author
---|---|---


***

### SAP SuccessFactors Employee Central
Recipe|Description|Author
---|---|---
[SAP SuccessFactors Employee Central Payroll Integration with SAP S_4HANA or SAP ERP](for/sapsuccessfactorsemployeecentralpayrollintegrationwithsaps4hanaorsaperp)| Replication of Payroll posting data from SAP SuccessFactors Employee Central to SAP ERP or SAP S/4HANA. This data includes Cost Center/GL accounts/Expenses.|[SAP API Business Hub](author.md#sap-api-business-hub)
[SAP SuccessFactors Employee Central with Third-Party Payroll Vendor](for/sapsuccessfactorsemployeecentralwiththirdpartypayrollvendor)| Integration of business processes in SAP SuccessFactors Employee Central system with Third Party Payroll Vendor; support for delta based integration with seperate files required for HIRE/REHIRE, Daily Changes and TERMINATION|[SAP API Business Hub](author.md#sap-api-business-hub)


***
### Security
Recipe|Description|Author
---|---|---
[Accessing keystore artifacts using a Groovy script](for/AccessTenantKeystoreusingScript) |Any keypair available in tenant keystore can be accessed programmatically from a script with the help of the getKey and getCertificate api of the KeyStoreService class.|[Shweta Walaskar](author.md#shweta-walaskar)|
[CMS Decryption with AES256-GCM algorithm using iaik libraries](for/Decryption_using_AES_GCM_iaik)|Decryption algorithm AES256-GCM using iaik which is the default security provider for CPI.|[Shweta Walaskar](author.md#shweta-walaskar)|
[Encryption with AES256-GCM algorithm using iaik libraries](for/Encryption_using_AES_GCM_iaik)|Encryption algorithm AES256-GCM using iaik which is the default security provider for CPI.|[Shweta Walaskar](author.md#shweta-walaskar)|
[Generate AWS4-HMAC-SHA256 Signature](for/GenerateAWS4_HMAC_SHA256)| A reusable recipe to generate an AWS specific AWS4-HMAC-SHA256 signature and pass it as a HTTP Authorization header.|[Sunny Kapoor](author.md#sunny-kapoor)|

***

### Third-Party Integrations

Recipe|Description|Author
---|---|---
[ SAP Ariba Integration with Third-Party for Analytical Reporting](for/saparibaanalyticalreportingintegrationwiththirdparty)| Consumption of Ariba APIs (Job Submission API and Job Results API) for Analytical Reporting ( Standard/Custom Templates) with CSV Output for integrating with Third Party  |[SAP API Business Hub](author.md#sap-api-business-hub)
[SAP Ariba Integration with Third-Party for Vendor And Questionnaires](for/saparibaintegrationwiththirdpartyforvendorandquestionnaires)| Ariba APIs for Vendor and Questionnaires with CSV Output for integrating with Third Party| [SAP API Business Hub](author.md#sap-api-business-hub)
[SAP Business Network Integration with Non-SAP ERP](for/sapbusinessnetworkintegrationwithnonsaperp)| Baseline template to support the Purchase Order, Invoice and other transactional documents with the SAP Business Network|[SAP API Business Hub](author.md#sap-api-business-hub)
[SAP SuccessFactors Employee Central with Third-Party Payroll Vendor](for/sapsuccessfactorsemployeecentralwiththirdpartypayrollvendor)| Integration of business processes in SAP SuccessFactors Employee Central system with Third Party Payroll Vendor; support for delta based integration with seperate files required for HIRE/REHIRE, Daily Changes and TERMINATION|[SAP API Business Hub](author.md#sap-api-business-hub)
