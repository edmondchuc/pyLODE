Markdown documentation created by [pyLODE](http://github.com/rdflib/pyLODE) 2.4

# {no title found}

## Metadata
* **IRI**
  * `http://linked.data.gov.au/def/agrif`
* **Publisher(s)**
  * [Department of Finance](http://linked.data.gov.au/org/finance)
* **Creators(s)**
  * John Machin of [Department of Finance](https://www.finance.gov.au)
  * Katherine Stuart of [Department of Finance](https://www.finance.gov.au)
  * [Armin Haller](http://orcid.org/0000-0003-3425-0780)
    [[ORCID]](http://orcid.org/0000-0003-3425-0780)
    (<armin.haller@anu.edu.au></a>) of [Australian National University](https://www.anu.edu.au)
* **Contributor(s)**
  * Kerry Taylor
  * Pouya Ghiasnezhad Omran
  * Sergio José Rodríguez Méndez
  * [Nicholas J. Car](http://orcid.org/0000-0002-8742-7730)
    [[ORCID]](http://orcid.org/0000-0002-8742-7730)
    (<nicholas.car@surroundaustralia.com></a>)
* **Created**
  * 2016-12-06
* **Modified**
  * 2019-10-21
* **Version Information**
  * 0.9
* **License &amp; Rights**
  * [https://creativecommons.org/licenses/by/4.0/](https://creativecommons.org/licenses/by/4.0/)
  * (c) Commonwealth of Australia (Department of Finance) 2019
* **Ontology RDF**
  * RDF ([agrif-notitle.ttl](turtle))
### Description
<p>The Australian Government Records Interoperability Framework (AGRIF, ‘the Framework’) is a system of related semantic ontologies that describe the structure, functions, and activities of the Australian Government, providing sufficient context for the effective use – including but not limited to management – of Australian Government information assets. It complies with the World Wide Web Consortium’s Web Ontology Language (OWL2) Recommendation and makes reference to other Recommendations and existing domain ontologies for archival and preservation processes.</p>

## Table of Contents
1. [Classes](#classes)
1. [Object Properties](#objectproperties)
1. [Datatype Properties](#datatypeproperties)
1. [Annotation Properties](#annotationproperties)
1. [Named Individuals](#namedindividuals)
1. [Namespaces](#namespaces)
1. [Legend](#legend)


## Overview

**Figure 1:** Ontology overview
## Classes
[AGIFT Function](#AGIFTFunction),
[Access Activity](#AccessActivity),
[Access Control](#AccessControl),
[Access Trigger](#AccessTrigger),
[Activity](#Activity),
[Administrator](#Administrator),
[Agent](#Agent),
[Artefact](#Artefact),
[Artefact Change Event](#ArtefactChangeEvent),
[Artefact Control Event](#ArtefactControlEvent),
[Artefact Publish Event](#ArtefactPublishEvent),
[Artefact Send Event](#ArtefactSendEvent),
[Artefact Share Event](#ArtefactShareEvent),
[Association](#Association),
[Business Owner](#BusinessOwner),
[Classifier](#Classifier),
[Collection](#Collection),
[Control](#Control),
[Controlled Vocabulary](#ControlledVocabulary),
[Coverage](#Coverage),
[Creator](#Creator),
[Decision Status](#DecisionStatus),
[Digital Artefact](#DigitalArtefact),
[Digital Holding Space](#DigitalHoldingSpace),
[Digital Preservation Policy](#DigitalPreservationPolicy),
[Disposal Class](#DisposalClass),
[Event](#Event),
[Form Factor](#FormFactor),
[Function](#Function),
[Holding Space](#HoldingSpace),
[Information Management Policy](#InformationManagementPolicy),
[Information System](#InformationSystem),
[Intellectual Control System](#IntellectualControlSystem),
[Jurisdictional Coverage](#JurisdictionalCoverage),
[Logical Collection](#LogicalCollection),
[Maintain Activity](#MaintainActivity),
[Manifest](#Manifest),
[Minimum Metadata Set Policy](#MinimumMetadataSetPolicy),
[Organisation](#Organisation),
[Organisational Unit](#OrganisationalUnit),
[Person](#Person),
[Physical Artefact](#PhysicalArtefact),
[Physical Collection](#PhysicalCollection),
[Physical Holding Space](#PhysicalHoldingSpace),
[Policy](#Policy),
[Preservation Quality](#PreservationQuality),
[Quality](#Quality),
[Record](#Record),
[Record Audit Event](#RecordAuditEvent),
[Record Control Event](#RecordControlEvent),
[Record Creation Event](#RecordCreationEvent),
[Record Decision Event](#RecordDecisionEvent),
[Record Destruction Event](#RecordDestructionEvent),
[Record Disposal Event](#RecordDisposalEvent),
[Record Freeze Event](#RecordFreezeEvent),
[Record Replacement Event](#RecordReplacementEvent),
[Record Sentencing Event](#RecordSentencingEvent),
[Record Storage Standard](#RecordStorageStandard),
[Record Transfer Event](#RecordTransferEvent),
[Records Authority Disposal Class Policy](#RecordsAuthorityDisposalClassPolicy),
[Records Authority Function](#RecordsAuthorityFunction),
[Role](#Role),
[Security Classification](#SecurityClassification),
[Security Clearance](#SecurityClearance),
[Security Control](#SecurityControl),
[Series](#Series),
[Share Activity](#ShareActivity),
[Spatial Coverage](#SpatialCoverage),
[Spatial Location](#SpatialLocation),
[Status](#Status),
[Temporal Coverage](#TemporalCoverage),
[Trigger](#Trigger),
[User](#User),
[Version History](#VersionHistory),
### AGIFT Function
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#AGIFTFunction`
Is Defined By | https://data.naa.gov.au/def/agift/
Description | <p>An AGIFT Function is a Function that classifies a Record according to the Australian Governments' Interactive Functions Thesaurus.</p>
Super-classes |[Function](Function) (c)<br />
### Access Activity
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#AccessActivity`
Description | <p>An Access Activity is an Activity where a Record is accessed by an Agent over a period of time.</p>
Super-classes |[Activity](Activity) (c)<br />
Restrictions |[triggers](triggers) (op) **only** [AccessTrigger](AccessTrigger) (c)<br />[accessedBy](accessedBy) (op) **some** [Agent](Agent) (c)<br />
### Access Control
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#AccessControl`
Description | <p>Access Control is the selective restriction of access to a Record or Artefact.</p>
Super-classes |[Control](Control) (c)<br />
Sub-classes |[SecurityClassification](SecurityClassification) (c)<br />
### Access Trigger
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#AccessTrigger`
Description | <p>An Access Trigger is a Trigger that can be initiated when a Record is accessed.</p>
Super-classes |[Trigger](Trigger) (c)<br />
### Activity
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#Activity`
Source | [https://www.w3.org/TR/prov-o/#Activity](https://www.w3.org/TR/prov-o/#Activity)
Description | <p>An Activity is something that occurs over a period of time on a Record.</p>
Restrictions |[guidingPolicy](guidingPolicy) (op) **only** [Policy](Policy) (c)<br />[requiresSecurityClassification](requiresSecurityClassification) (op) **only** [SecurityClassification](SecurityClassification) (c)<br />[associatedFunction](associatedFunction) (op) **only** [Function](Function) (c)<br />[wasAssociatedWith](wasAssociatedWith) (op) **some** [Agent](Agent) (c)<br />[qualifiedAssociation](qualifiedAssociation) (op) **some** [Association](Association) (c)<br />[endedAtTime](endedAtTime) (dp) **max** 1<br />[hasLocation](hasLocation) (op) **only** [SpatialLocation](SpatialLocation) (c)<br />[usedRecord](usedRecord) (op) **only** [Record](Record) (c)<br />[hasStatus](hasStatus) (op) **only** [Status](Status) (c)<br />[startedAtTime](startedAtTime) (dp) **max** 1<br />
Sub-classes |[AccessActivity](AccessActivity) (c)<br />[ShareActivity](ShareActivity) (c)<br />[MaintainActivity](MaintainActivity) (c)<br />
### Administrator
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#Administrator`
Description | <p>An Administrator is a Role that has overall responsibility for the administration and functions of an Information System, but not necessarily for the information stored within.</p>
Super-classes |[Role](Role) (c)<br />
### Agent
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#Agent`
Source | [https://www.w3.org/TR/prov-o/#Agent](https://www.w3.org/TR/prov-o/#Agent)
Description | <p>An Agent is a corporate entity, organisational element or system, or individual responsible for the performance of some Activity or Event, including those on Records.</p>
Restrictions |[hasPermission](hasPermission) (op) **some** [Permission](SecurityClearance) (c)<br />[actsAs](actsAs) (op) **some** [Role](Role) (c)<br />[positionIn](positionIn) (op) **some** [Organisation](Organisation) (c)<br />
Sub-classes |[Person](Person) (c)<br />[Organisation](Organisation) (c)<br />
### Artefact
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#Artefact`
Description | <p>An Artefact is an object that is made by a Person and that is to be preserved.</p>
Restrictions |[softwareAssignedID](softwareAssignedID) (dp) **some** [xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />[isAffectedBy](isAffectedBy) (op) **some** [Event](Event) (c)<br />[storedIn](storedIn) (op) **some** [IntellectualControlSystem](IntellectualControlSystem) (c)<br />[hasQuality](hasQuality) (op) **some** [PreservationQuality](PreservationQuality) (c)<br />[isChangedBy](isChangedBy) (op) **some** [InformationSystem](InformationSystem) (c)<br />[relatedTo](relatedTo) (op) **only** [Artefact](Artefact) (c)<br />[requiresSecurityClassification](requiresSecurityClassification) (op) **only** [SecurityClassification](SecurityClassification) (c)<br />[hasLocation](hasLocation) (op) **only** [SpatialLocation](SpatialLocation) (c)<br />
Sub-classes |[DigitalArtefact](DigitalArtefact) (c)<br />[PhysicalArtefact](PhysicalArtefact) (c)<br />
### Artefact Change Event
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#ArtefactChangeEvent`
Description | <p>An Artefact Change Event is an Event that results in a new version of an Artefact.</p>
Super-classes |[Event](Event) (c)<br />
Restrictions |[affects](affects) (op) **min** 2 [Artefact](Artefact) (c)<br />
Sub-classes |[ArtefactSendEvent](ArtefactSendEvent) (c)<br />
### Artefact Control Event
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#ArtefactControlEvent`
Description | <p>An Artefact Control Event is an Event that requires a particular level of access to an Artefact.</p>
Super-classes |[Event](Event) (c)<br />
Restrictions |[hasControl](requiresControl) (op) **only** [Control](Control) (c)<br />
Sub-classes |[ArtefactShareEvent](ArtefactShareEvent) (c)<br />[ArtefactPublishEvent](ArtefactPublishEvent) (c)<br />
### Artefact Publish Event
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#ArtefactPublishEvent`
Description | <p>An Artefact Publish Event is an Event that gives indiscriminate access to an Artefact to a set of Agents.</p>
Super-classes |[ArtefactControlEvent](ArtefactControlEvent) (c)<br />
### Artefact Send Event
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#ArtefactSendEvent`
Description | <p>An Artefact Send Event is an Event that results in a new version or a set of new versions of an Artefact at a target Agent or a set of target Agents.</p>
Super-classes |[ArtefactChangeEvent](ArtefactChangeEvent) (c)<br />
Restrictions |[hasTargetAgent](hasTargetAgent) (op) **min** 1 [Agent](Agent) (c)<br />[hasSourceAgent](hasSourceAgent) (op) **exactly** 1 [Agent](Agent) (c)<br />
### Artefact Share Event
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#ArtefactShareEvent`
Description | <p>An Artefact Share Event is an Event that gives access to an Artefact to an Agent or a defined set of Agents.</p>
Super-classes |[ArtefactControlEvent](ArtefactControlEvent) (c)<br />
Restrictions |[hasSourceAgent](hasSourceAgent) (op) **exactly** 1 [Agent](Agent) (c)<br />[hasTargetAgent](hasTargetAgent) (op) **min** 1 [Agent](Agent) (c)<br />
### Association
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#Association`
Source | [https://www.w3.org/TR/prov-o/#Association](https://www.w3.org/TR/prov-o/#Association)
Description | <p>An Association is a qualified assignment of responsibility to an Agent in an Activity or Event, indicating that the Agent had a Role in the Activity.</p>
Restrictions |[hasAgent](hasAgent) (op) **only** [Agent](Agent) (c)<br />[associatedRole](associatedRole) (op) **only** [Role](Role) (c)<br />
### Business Owner
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#BusinessOwner`
Description | <p>A Business Owner is the Role that has the managerial control of a Function.</p>
Super-classes |[Role](Role) (c)<br />
### Classifier
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#Classifier`
Description | <p>A Classifier is a machine-generated and applied category that a set of Records belong to.</p>
Restrictions |[associatedFunction](associatedFunction) (op) **only** [Function](Function) (c)<br />
### Collection
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#Collection`
Description | <p>A Collection is an aggregation of Artefact items.</p>
Restrictions |[hasPart](hasPart) (op) **some** [Artefact](Artefact) (c)<br />
Sub-classes |[PhysicalCollection](PhysicalCollection) (c)<br />[LogicalCollection](LogicalCollection) (c)<br />
### Control
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#Control`
Description | <p>A Control is a security or access measure that safeguards or restricts access to an asset.</p>
Sub-classes |[AccessControl](AccessControl) (c)<br />[SecurityControl](SecurityControl) (c)<br />
### Controlled Vocabulary
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#ControlledVocabulary`
Description | <p>A Controlled Vocabulary is an Intellectual Control System that provides a way to organize Records that facilitates a later discovery of a Record.</p>
Super-classes |[IntellectualControlSystem](IntellectualControlSystem) (c)<br />
Restrictions |[associatedFunction](associatedFunction) (op) **only** [Function](Function) (c)<br />
### Coverage
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#Coverage`
Description | <p>A Coverage denotes the jurisdictional applicability, or the temporal and/or spatial extent to which a Record is observed.</p>
Sub-classes |[TemporalCoverage](TemporalCoverage) (c)<br />[JurisdictionalCoverage](JurisdictionalCoverage) (c)<br />[SpatialCoverage](SpatialCoverage) (c)<br />
### Record Creation Event
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#CreationEvent`
Description | <p>A Record Creation Event is an Event that results in the creation of a Record.</p>
Super-classes |[Event](Event) (c)<br />
### Creator
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#Creator`
Description | <p>A Creator is the Agent that has created a Record or Artefact.</p>
Super-classes |[Role](Role) (c)<br />
### Decision Status
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#DecisionStatus`
Description | <p>A Decision Status is a Status that indicates the approval or disapproval of a Decision Event.</p>
Super-classes |[Status](Status) (c)<br />
### Digital Artefact
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#DigitalArtefact`
Description | <p>A Digital Artefact is an Artefact that is of a digital nature and stored in an Information System.</p>
Super-classes |[Artefact](Artefact) (c)<br />
Restrictions |[filesize](filesize) (dp) **some** [xsd:long](http://www.w3.org/2001/XMLSchema#long) (c)<br />[filename](filename) (dp) **some** [rdfs:Literal](http://www.w3.org/2000/01/rdf-schema#Literal) (c)<br />[format](format) (dp) **some** [rdfs:Literal](http://www.w3.org/2000/01/rdf-schema#Literal) (c)<br />[storedIn](storedIn) (op) **some** [InformationSystem](InformationSystem) (c)<br />
### Digital Holding Space
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#DigitalHoldingSpace`
Description | <p>A Digital Holding Space is a space that is used or reserved for the storage of a Digital Artefact on a storage medium or virtual storage space.</p>
Super-classes |[HoldingSpace](HoldingSpace) (c)<br />
### Digital Preservation Policy
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#DigitalPreservationPolicy`
Description | <p>The Digital Preservation Policy defines the process of active management by which the National Archives ensures that a digital object will be accessible in the future.</p>
Super-classes |[Policy](Policy) (c)<br />
### Disposal Class
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#DisposalClass`
Description | <p>A Disposal Class is a Policy that defines the sentencing requirements of an item.</p>
Super-classes |[RecordsAuthorityPolicy](RecordsAuthorityDisposalClassPolicy) (c)<br />
Restrictions |[disposalClassNumber](disposalClassNumber) (dp) **exactly** 1<br />
### Event
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#Event`
Source | [https://www.w3.org/TR/prov-o/#InstantaneousEvent](https://www.w3.org/TR/prov-o/#InstantaneousEvent)
Description | <p>An Event denotes an instantaneous transition in the world.</p>
Restrictions |[triggeredBy](triggeredBy) (op) **only** [Trigger](Trigger) (c)<br />[guidingPolicy](guidingPolicy) (op) **only** [Policy](Policy) (c)<br />[affects](affects) (op) **some** ([Artefact](Artefact) (c) or [Record](Record) (c))<br />[associatedFunction](associatedFunction) (op) **only** [Function](Function) (c)<br />[hasStatus](hasStatus) (op) **only** [Status](Status) (c)<br />[priorEvent](priorEvent) (op) **only** [Event](Event) (c)<br />[qualifiedAssociation](qualifiedAssociation) (op) **some** [Association](Association) (c)<br />[wasAssociatedWith](wasAssociatedWith) (op) **some** [Agent](Agent) (c)<br />
Sub-classes |[CreationEvent](RecordCreationEvent) (c)<br />[ArtefactChangeEvent](ArtefactChangeEvent) (c)<br />[ArtefactControlEvent](ArtefactControlEvent) (c)<br />[RecordControlEvent](RecordControlEvent) (c)<br />
### Form Factor
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#FormFactor`
Description | <p>A Form Factor defines and prescribes the size, shape, and other physical specifications of a Physical Artefact that is stored.</p>
### Function
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#Function`
Description | <p>A Function reflects the responsibilities of an Organisation that can be delegated through official channels. [Commonwealth Records Series Manual]</p>
Restrictions |[guidingPolicy](guidingPolicy) (op) **only** [Policy](Policy) (c)<br />
Sub-classes |[RecordsAuthorityFunction](RecordsAuthorityFunction) (c)<br />[AGIFTFunction](AGIFTFunction) (c)<br />
### Holding Space
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#HoldingSpace`
Description | <p>A Holding Space is a space that is used or reserved for the storage of an Artefact.</p>
Super-classes |[SpatialLocation](SpatialLocation) (c)<br />
Sub-classes |[DigitalHoldingSpace](DigitalHoldingSpace) (c)<br />[PhysicalHoldingSpace](PhysicalHoldingSpace) (c)<br />
### Information Management Policy
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#InformationManagementPolicy`
Description | <p>An Information Management Policy is a Policy that helps to align information management practices to fulfill the requirements of an information governance framework. An Information Management Policy provides direction and guidance to staff for creating, capturing and managing information to satisfy business, legal and stakeholder requirements, and assigns responsibilities across the agency.</p>
Super-classes |[Policy](Policy) (c)<br />
Restrictions |[hasDisposalClass](hasDisposalClass) (op) **only** [DisposalClass](DisposalClass) (c)<br />
### Information System
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#InformationSystem`
Description | <p>An Information System is an organized system for the collection, organization, storage and communication of information, typically Digital Artefacts or Records.</p>
Sub-classes |[IntellectualControlSystem](IntellectualControlSystem) (c)<br />
### Intellectual Control System
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#IntellectualControlSystem`
Description | <p>An Intellectual Control System is a System that enables Agents to locate and manage information.</p>
Super-classes |[InformationSystem](InformationSystem) (c)<br />
Restrictions |[guidingPolicy](guidingPolicy) (op) **only** [Policy](Policy) (c)<br />
Sub-classes |[ControlledVocabulary](ControlledVocabulary) (c)<br />[Series](Series) (c)<br />
### Jurisdictional Coverage
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#JurisdictionalCoverage`
Description | <p>A Jurisdictional Coverage denotes the jurisdictional applicability of the Record.</p>
Super-classes |[Coverage](Coverage) (c)<br />
### Logical Collection
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#LogicalCollection`
Description | <p>A Logical Collection is an aggregation of Artefact items that are stored within one physical file.</p>
Super-classes |[Collection](Collection) (c)<br />
### Maintain Activity
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#MaintainActivity`
Description | <p>A Maintain Activity is an Activity to maintain a Record over a period of time due to a BusinessFunction or Policy.</p>
Super-classes |[Activity](Activity) (c)<br />
Restrictions |[hasQuality](hasQuality) (op) **some** [PreservationQuality](PreservationQuality) (c)<br />
### Manifest
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#Manifest`
Description | <p>A Manifest describes the files involved in the transfer of a Record from an Agency to the National Archives, including details such as the filesize, the destination hierarchy and the file's metadata.</p>
Restrictions |[checksum](checksum) (dp) **exactly** 1<br />
### Minimum Metadata Set Policy
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#MinimumMetadataSetPolicy`
Description | <p>The Minimum Metadata Set Policy is a Policy that has been developed by the National Archives of Australia to identify metadata properties essential for agency management of information as well as those needed for records which will be transferred to the Archives. It supports the Digital Continuity 2020 principles of interoperable systems and processes and is a practical application of the Australian Government Recordkeeping Metadata Standard 2.2 (AGRkMS) to support metadata implementation and information use in agencies.</p>
Super-classes |[Policy](Policy) (c)<br />
### Organisation
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#Organisation`
Source | [https://www.w3.org/TR/prov-o/#Organization](https://www.w3.org/TR/prov-o/#Organization)
Description | <p>An Organisation is a type of Agent that denotes a social or legal institution such as a government agency, a corporation, society, etc.</p>
Super-classes |[Agent](Agent) (c)<br />
Restrictions |[associatedFunction](associatedFunction) (op) **some** [Function](Function) (c)<br />
Sub-classes |[OrganisationalUnit](OrganisationalUnit) (c)<br />
### Organisational Unit
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#OrganisationalUnit`
Description | <p>An Organisational Unit is a division of labour typically organised around a business function that form part of the Organisation.</p>
Super-classes |[Organisation](Organisation) (c)<br />
Restrictions |[partOf](partOf) (op) **only** [Organisation](Organisation) (c)<br />
### Security Clearance
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#Permission`
Source | Australian Government Recordkeeping Metadata Standard
Description | <p>A Permission denotes the Security Clearance of an Agent that determines its access and use rights.</p>
### Person
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#Person`
Source | [https://www.w3.org/TR/prov-o/#Person](https://www.w3.org/TR/prov-o/#Person)
Description | <p>A Person is an Agent that denotes a human.</p>
Super-classes |[Agent](Agent) (c)<br />
### Physical Artefact
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#PhysicalArtefact`
Description | <p>A Physical Artefact is an Artefact that is of physical nature.</p>
Example | `An example of a Phyiscal Artefact in the context of record keeping is information printed or written on paper.`<br />
Super-classes |[Artefact](Artefact) (c)<br />
Restrictions |[hasFormFactor](hasFormFactor) (op) **only** [FormFactor](FormFactor) (c)<br />
### Physical Collection
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#PhysicalCollection`
Description | <p>A Physical Collection is an aggregation of Artefact items that are stored in separate physical files.</p>
Super-classes |[Collection](Collection) (c)<br />
### Physical Holding Space
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#PhysicalHoldingSpace`
Description | <p>A Physical Holding Space is a Spatial Location that is used or reserved for the storage of a Physical Artefact.</p>
Super-classes |[HoldingSpace](HoldingSpace) (c)<br />
### Policy
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#Policy`
Source | [dcterms:Policy](http://purl.org/dc/terms/Policy)
Description | <p>A Policy is a deliberate system of principles to guide decisions and achieve rational outcomes.</p>
Sub-classes |[RecordStorageStandard](RecordStorageStandard) (c)<br />[MinimumMetadataSetPolicy](MinimumMetadataSetPolicy) (c)<br />[RecordsAuthorityPolicy](RecordsAuthorityDisposalClassPolicy) (c)<br />[DigitalPreservationPolicy](DigitalPreservationPolicy) (c)<br />[InformationManagementPolicy](InformationManagementPolicy) (c)<br />
### Preservation Quality
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#PreservationQuality`
Description | <p>A Preservation Quality describes a Quality of an Artefact that supports or threatens the long term preservation of the information that is to be preserved.</p>
Super-classes |[Quality](Quality) (c)<br />
### Quality
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#Quality`
Description | <p>A Quality is an attribute that is intrinsically associated with an entity.</p>
Sub-classes |[PreservationQuality](PreservationQuality) (c)<br />
### Record
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#Record`
Description | <p>A Record is information in any format created, received and maintained as evidence by an Organisation or Person, in pursuance of legal obligations or in the transaction of business. A Record may comprise a Digital or Physical Artefact.</p>
Restrictions |[hasActivity](hasActivity) (op) **only** [Activity](Activity) (c)<br />[hasClassifier](hasClassifier) (op) **some** [Classifier](Classifier) (c)<br />[isAffectedBy](isAffectedBy) (op) **only** [Event](Event) (c)<br />[checksum](checksum) (dp) **max** 1<br />[recordOf](recordOf) (op) **min** 1 [Artefact](Artefact) (c)<br />[hasCoverage](hasCoverage) (op) **only** [Coverage](Coverage) (c)<br />[hasDisposalClass](hasDisposalClass) (op) **exactly** 1 [DisposalClass](DisposalClass) (c)<br />[isAffectedBy](isAffectedBy) (op) **exactly** 1 [CreationEvent](RecordCreationEvent) (c)<br />[hasSeries](hasSeries) (op) **only** [Series](Series) (c)<br />[associatedFunction](associatedFunction) (op) **min** 1 [Function](Function) (c)<br />[qualifiedAssociation](qualifiedAssociation) (op) **some** [Association](Association) (c)<br />[relatedTo](relatedTo) (op) **only** [Record](Record) (c)<br />[hasControl](requiresControl) (op) **only** [Control](Control) (c)<br />[hasStatus](hasStatus) (op) **only** [Status](Status) (c)<br />[requiresSecurityClassification](requiresSecurityClassification) (op) **only** [SecurityClassification](SecurityClassification) (c)<br />[replaces](replaces) (op) **only** [Record](Record) (c)<br />
### Record Audit Event
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#RecordAuditEvent`
Description | <p>An Record Audit Event is the systematic examination of a Record to ascertain how and where the Record is stored, who created it, or manages it, who uses it and how much longer the Record is required to be maintained.</p>
Super-classes |[RecordControlEvent](RecordControlEvent) (c)<br />
### Record Control Event
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#RecordControlEvent`
Description | <p>A Record Control Event is an Event that requires a particular level of access to the Record.</p>
Super-classes |[Event](Event) (c)<br />
Restrictions |[hasControl](requiresControl) (op) **only** [Control](Control) (c)<br />
Sub-classes |[RecordDecisionEvent](RecordDecisionEvent) (c)<br />[RecordReplacementEvent](RecordReplacementEvent) (c)<br />[RecordAuditEvent](RecordAuditEvent) (c)<br />[RecordDisposalEvent](RecordDisposalEvent) (c)<br />[RecordSentencingEvent](RecordSentencingEvent) (c)<br />
### Record Decision Event
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#RecordDecisionEvent`
Description | <p>A Record Decision Event changes the Decision Status on the Control of a Record.</p>
Super-classes |[RecordControlEvent](RecordControlEvent) (c)<br />
Restrictions |[hasPrerequisiteDecisionEvent](prerequisiteDecisionEvent) (op) **only** [RecordDecisionEvent](RecordDecisionEvent) (c)<br />[hasDecisionStatus](hasDecisionStatus) (op) **only** [DecisionStatus](DecisionStatus) (c)<br />
### Record Destruction Event
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#RecordDestructionEvent`
Description | <p>A Record Destruction Event is a Disposal Event that results in the regular authorised permanent desctruction of a Record that is no longer required for business purposes.</p>
Super-classes |[RecordDisposalEvent](RecordDisposalEvent) (c)<br />
### Record Disposal Event
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#RecordDisposalEvent`
Description | <p>A Record Disposal Event is an Event that results in the regular authorised destruction or change of custody of a Record that is no longer required for business purposes.</p>
Super-classes |[RecordControlEvent](RecordControlEvent) (c)<br />
Sub-classes |[RecordFreezeEvent](RecordFreezeEvent) (c)<br />[RecordDestructionEvent](RecordDestructionEvent) (c)<br />[RecordTransferEvent](RecordTransferEvent) (c)<br />
### Record Freeze Event
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#RecordFreezeEvent`
Description | <p>A Record Freeze Event is a Disposal Event that leads to a records disposal freeze or retention notice in support of compliance requirements or an identified need to suspend the Archives' records destruction permissions.</p>
Super-classes |[RecordDisposalEvent](RecordDisposalEvent) (c)<br />
### Record Replacement Event
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#RecordReplacementEvent`
Description | <p>A Record Replacement Event is an Event that results in the replacement of a Record with a new version. Edits to a Record constitute a Replace Event.</p>
Super-classes |[RecordControlEvent](RecordControlEvent) (c)<br />
Restrictions |[replacedBy](replacedBy) (op) **exactly** 1 [Record](Record) (c)<br />[hasVersionHistory](hasVersionHistory) (op) **only** [VersionHistory](VersionHistory) (c)<br />
### Record Sentencing Event
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#RecordSentencingEvent`
Description | <p>A Record Sentencing Event is an Event that classifies an Agencies Record to a specific class of a Records Authority Disposal Class Policy. This helps determine the Records value and how it should be managed throughout its lifecycle.</p>
Super-classes |[RecordControlEvent](RecordControlEvent) (c)<br />
### Record Storage Standard
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#RecordStorageStandard`
Description | <p>The Standard for the storage of non-digital archival Records is designed to set out the requirements for the safe storage and preservation of non-digital records in the Archives’ custody; to ensure all non-digital records are protected, secure and accessible for as long as they are required to meet business and accountability needs and community expectations; and to ensure all non-digital records are stored in the most cost-effective manner possible.</p>
Super-classes |[Policy](Policy) (c)<br />
### Record Transfer Event
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#RecordTransferEvent`
Description | <p>A Transfer Event is a Disposal Event that results in a change of custody.</p>
Example | `An example of a Record Transfer Event is the transfer of a Record from an Agency to the National Archives. Section 27 of the Archives Act 1983 requires Australian government agencies to transfer Records to the Archives within 15 years of their creation.`<br />
Super-classes |[RecordDisposalEvent](RecordDisposalEvent) (c)<br />
Restrictions |[hasManifest](hasManifest) (op) **only** [Manifest](Manifest) (c)<br />[transferredTo](transferredTo) (op) **some** [Role](Role) (c)<br />[transferredFrom](transferredFrom) (op) **some** [Role](Role) (c)<br />
### Records Authority Function
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#RecordsAuthorityFunction`
Description | <p>A Records Authority Function is a Function that is assigned by the National Archives to classify Agency business.</p>
Super-classes |[Function](Function) (c)<br />
### Records Authority Disposal Class Policy
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#RecordsAuthorityPolicy`
Source | Australian Government Recordkeeping Metadata Standard
Description | <p>A Records Authority Disposal Class Policy is a Policy that identifies the specific disposal class that authorises the retention or destruction of a Record.</p>
Super-classes |[Policy](Policy) (c)<br />
Restrictions |[hasDisposalClass](hasDisposalClass) (op) **exactly** 1 [DisposalClass](DisposalClass) (c)<br />
Sub-classes |[DisposalClass](DisposalClass) (c)<br />
### Role
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#Role`
Source | [https://www.w3.org/TR/prov-o/#Role](https://www.w3.org/TR/prov-o/#Role)
Description | <p>A Role is the function of an entity or agent with respect to an Activity or Event, in the context of a usage, generation, invalidation, association, start, and end.</p>
Restrictions |[hasPermission](hasPermission) (op) **some** [Permission](SecurityClearance) (c)<br />
Sub-classes |[BusinessOwner](BusinessOwner) (c)<br />[User](User) (c)<br />[Creator](Creator) (c)<br />[Administrator](Administrator) (c)<br />
### Security Classification
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#SecurityClassification`
Source | Australian Government Recordkeeping Metadata Standard
Description | <p>A Security Classification denotes the security status of a Record that an Agent needs to possess to access the Record.</p>
Super-classes |[AccessControl](AccessControl) (c)<br />
### Security Control
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#SecurityControl`
Description | <p>A Security Control is a safeguard or countermeasures to avoid, detect, counteract, or minimize security risks to a Record or Artefact.</p>
Super-classes |[Control](Control) (c)<br />
### Series
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#Series`
Description | <p>A Series is an identifier for an item, and when combined with a control symbol gives an item its intellectual context.</p>
Super-classes |[IntellectualControlSystem](IntellectualControlSystem) (c)<br />
Restrictions |[associatedFunction](associatedFunction) (op) **only** [Function](Function) (c)<br />
### Share Activity
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#ShareActivity`
Description | <p>A Share Activity is an Activity where the custodianship of a Record is transferred to or shared with Agents over a period of time.</p>
Super-classes |[Activity](Activity) (c)<br />
Restrictions |[sharedWith](sharedWith) (op) **some** [Agent](Agent) (c)<br />
### Spatial Coverage
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#SpatialCoverage`
Description | <p>A Spatial Coverage denotes the spatial extent to which a Record is observed.</p>
Super-classes |[Coverage](Coverage) (c)<br />
### Spatial Location
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#SpatialLocation`
Description | <p>A Spatial Location describes where a something (e.g. a Record, Collection or Artefact) is physically located, using geospatial coordinates such as latitude and longitude.</p>
Sub-classes |[HoldingSpace](HoldingSpace) (c)<br />
### Status
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#Status`
Description | <p>A Status indicates an Activities current state.</p>
Sub-classes |[DecisionStatus](DecisionStatus) (c)<br />
### Temporal Coverage
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#TemporalCoverage`
Description | <p>A Temporal Coverage denotes the temporal extent to which a Record is observed.</p>
Super-classes |[Coverage](Coverage) (c)<br />
### Trigger
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#Trigger`
Description | <p>A Trigger is an entity that initiated an Activity or Event.</p>
Restrictions |[notifies](notifies) (op) **some** [Agent](Agent) (c)<br />
Sub-classes |[AccessTrigger](AccessTrigger) (c)<br />
### User
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#User`
Description | <p>A User is an Agent that uses a Record.</p>
Super-classes |[Role](Role) (c)<br />
### Version History
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#VersionHistory`
Description | <p>A Version History is the cumulative change to a previous version of a file.</p>

## Object Properties
[accessed By](#accessedBy),
[acts As](#actsAs),
[affects](#affects),
[associated Function](#associatedFunction),
[associated Role](#associatedRole),
[guiding Policy](#guidingPolicy),
[has Activity](#hasActivity),
[has Agent](#hasAgent),
[has Classifier](#hasClassifier),
[requires Control](#requiresControl),
[has Coverage](#hasCoverage),
[has Decision Status](#hasDecisionStatus),
[has Disposal Class](#hasDisposalClass),
[has Form Factor](#hasFormFactor),
[has Location](#hasLocation),
[has Manifest](#hasManifest),
[has Next Version](#hasNextVersion),
[has Part](#hasPart),
[has Permission](#hasPermission),
[prerequisite Decision Event](#prerequisiteDecisionEvent),
[has Previous Version](#hasPreviousVersion),
[has Quality](#hasQuality),
[has Series](#hasSeries),
[has Source Agent](#hasSourceAgent),
[has Status](#hasStatus),
[has Target Agent](#hasTargetAgent),
[has Version History](#hasVersionHistory),
[is Affected By](#isAffectedBy),
[is Attached To](#isAttachedTo),
[is Based On](#isBasedOn),
[is Changed By](#isChangedBy),
[is Duplicate Of](#isDuplicateOf),
[is Mentioned In](#isMentionedIn),
[is Part Of](#isPartOf),
[notifies](#notifies),
[part Of](#partOf),
[position In](#positionIn),
[prior Event](#priorEvent),
[qualified Association](#qualifiedAssociation),
[record Of](#recordOf),
[related To](#relatedTo),
[replaced By](#replacedBy),
[replaces](#replaces),
[requires Security Classification](#requiresSecurityClassification),
[shared With](#sharedWith),
[stored In](#storedIn),
[transferred From](#transferredFrom),
[transferred To](#transferredTo),
[triggered By](#triggeredBy),
[triggers](#triggers),
[used Record](#usedRecord),
[was Associated With](#wasAssociatedWith),
[](accessedBy)
### accessed By
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#accessedBy`
Description | A relation that indicates that an Agent has accessed a Record as defined in an Access Activity.
Super-properties |[wasAssociatedWith](wasAssociatedWith) (op)<br />
[](actsAs)
### acts As
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#actsAs`
Description | A relation between an Agent and the Role that Agent acts in.
[](affects)
### affects
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#affects`
Description | A relation between an Event and an Artefact or a Record.
[](associatedFunction)
### associated Function
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#associatedFunction`
Description | A relation that associates a Function to an Entity, Event or Activity.
[](associatedRole)
### associated Role
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#associatedRole`
Source | [https://www.w3.org/TR/prov-o/#hadRole](https://www.w3.org/TR/prov-o/#hadRole)
Description | An associated Role is a qualified association between a Role and an Activity or Event defined by an Association.
[](guidingPolicy)
### guiding Policy
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#guidingPolicy`
Description | A relation that defines a Policy that is guiding an Activity or Change Event.
[](hasActivity)
### has Activity
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#hasActivity`
Source | [https://www.w3.org/TR/prov-o/#p_activity](https://www.w3.org/TR/prov-o/#p_activity)
Description | A relation between a Record and an Activity that acts upon the Record.
[](hasAgent)
### has Agent
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#hasAgent`
Source | [https://www.w3.org/TR/prov-o/#p_agent](https://www.w3.org/TR/prov-o/#p_agent)
Description | A qualified relation between an Agent and a Change Event defined through an Association.
[](hasClassifier)
### has Classifier
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#hasClassifier`
Super-properties |[owl:topObjectProperty](http://www.w3.org/2002/07/owl#topObjectProperty)<br />
[](requiresControl)
### requires Control
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#hasControl`
Description | A relation between a Record, Artefact or Event and a Control that denotes the required level of Access or Security Control.
[](hasCoverage)
### has Coverage
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#hasCoverage`
Description | A relation between a Record and its Jurisdictional Coverage, or its Temporal or Spatial Coverage.
[](hasDecisionStatus)
### has Decision Status
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#hasDecisionStatus`
Description | A relation that indicates what the Decision on a Decision Event was.
[](hasDisposalClass)
### has Disposal Class
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#hasDisposalClass`
Description | A relation that associates a Disposal Class with a Record.
[](hasFormFactor)
### has Form Factor
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#hasFormFactor`
Description | A relation that defines the size, shape, and other physical specifications of a Physical Artefact.
[](hasLocation)
### has Location
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#hasLocation`
Description | A relation that defines the Spatial Location of an Activity or Artefact.
[](hasManifest)
### has Manifest
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#hasManifest`
Description | A relation between a Manifest and a Transfer Event that describes the files involved in the transfer of a Record.
[](hasNextVersion)
### has Next Version
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#hasNextVersion`
Description | A relation that indicates that an Artefact has a newer version.
Super-properties |[relatedTo](relatedTo) (op)<br />
[](hasPart)
### has Part
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#hasPart`
Description | A relation that defines part-whole relations.
[](hasPermission)
### has Permission
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#hasPermission`
Description | A relation between an Agent and the Permission the Agent possesses.
[](prerequisiteDecisionEvent)
### prerequisite Decision Event
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#hasPrerequisiteDecisionEvent`
Description | A relation between a Decision Event and a prerequisite Decision Event, indicating a Decision chain in a Chain of Command.
Super-properties |[priorEvent](priorEvent) (op)<br />
[](hasPreviousVersion)
### has Previous Version
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#hasPreviousVersion`
Description | A relation that indicates that an Artefact has an older version.
Super-properties |[relatedTo](relatedTo) (op)<br />
[](hasQuality)
### has Quality
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#hasQuality`
Description | A relation that indicates a specific Quality of an Artefact.
[](hasSeries)
### has Series
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#hasSeries`
Description | A relation between a Record and its Series Number.
Super-properties |[owl:topObjectProperty](http://www.w3.org/2002/07/owl#topObjectProperty)<br />
[](hasSourceAgent)
### has Source Agent
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#hasSourceAgent`
Description | A relation that denotes the source Agent of a Record or an Artefact in an Event or Activity.
Super-properties |[wasAssociatedWith](wasAssociatedWith) (op)<br />
[](hasStatus)
### has Status
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#hasStatus`
Description | A relation between an Activity and a Status that indicates its current state.
[](hasTargetAgent)
### has Target Agent
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#hasTargetAgent`
Description | A relation that denotes the target Agent of a Record or an Artefact in an Event or Activity.
Super-properties |[wasAssociatedWith](wasAssociatedWith) (op)<br />
[](hasVersionHistory)
### has Version History
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#hasVersionHistory`
Description | A relation between a Record and its previous Version qualified through a Replace Event.
[](isAffectedBy)
### is Affected By
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#isAffectedBy`
Description | A relation between an Artefact or a Record and an Event.
Super-properties |[owl:topObjectProperty](http://www.w3.org/2002/07/owl#topObjectProperty)<br />
[](isAttachedTo)
### is Attached To
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#isAttachedTo`
Description | A relation that indicates that an Artefact is logically or physically attached to another Artefact.
Super-properties |[relatedTo](relatedTo) (op)<br />
[](isBasedOn)
### is Based On
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#isBasedOn`
Description | A relation that indicates that an Artefact is in part or as a whole based on another Artefact.
Super-properties |[relatedTo](relatedTo) (op)<br />
[](isChangedBy)
### is Changed By
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#isChangedBy`
Description | A relation that denotes the Information System that has been used to change an Artefact.
[](isDuplicateOf)
### is Duplicate Of
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#isDuplicateOf`
Description | A relation that indicates that an Artefact is an exact copy of another Artefact, i.e. the content is exactly the same, but its Record may be different.
Super-properties |[relatedTo](relatedTo) (op)<br />
[](isMentionedIn)
### is Mentioned In
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#isMentionedIn`
Description | A relation that indicates that an Artefact is mentioned in another Artefact. An example of such a relation is a citation of a document in another document.
Super-properties |[relatedTo](relatedTo) (op)<br />
[](isPartOf)
### is Part Of
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#isPartOf`
Description | A Collection in which the described Artefact is physically or logically included.
[](notifies)
### notifies
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#notifies`
Description | A relation between a Trigger and an Agent that is to be notified.
[](partOf)
### part Of
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#partOf`
Description | A relation that defines part-whole relations.
[](positionIn)
### position In
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#positionIn`
Description | A relation that defines the position an Agent occupies in an Organisation or Organisational Unit.
[](priorEvent)
### prior Event
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#priorEvent`
Description | A relation indicating some causal link between an Event and a previously happening Event.
[](qualifiedAssociation)
### qualified Association
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#qualifiedAssociation`
Description | A relation that associates an assignment of responsibility to an Agent for an Activity or Event, indicating that the Agent had a Role in the Activity or Event.
[](recordOf)
### record Of
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#recordOf`
Description | A relation that defines what Artefact the Record is about.
[](relatedTo)
### related To
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#relatedTo`
Description | A relation that indicates that there is some form of relation between a Record and another Record or between an Artefact and another Artefact.
[](replacedBy)
### replaced By
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#replacedBy`
Description | A relation that defines that a Record has been replaced by another Record, qualified through a Replace Event.
[](replaces)
### replaces
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#replaces`
Description | A relation that defines that a Record replaces another Record, qualified through a Replace Event.
[](requiresSecurityClassification)
### requires Security Classification
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#requiresSecurityClassification`
Description | A relation between a Record and a Security Classification that denotes the required level of Security Clearance an Agent needs to possess to access the Record.
Super-properties |[hasControl](requiresControl) (op)<br />
[](sharedWith)
### shared With
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#sharedWith`
Description | A relation that indicates that a Record was shared with an Agent as defined in a Share Activity.
Super-properties |[wasAssociatedWith](wasAssociatedWith) (op)<br />
[](storedIn)
### stored In
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#storedIn`
Description | A relation that indicates the Storage Location of an Artefact.
Super-properties |[owl:topObjectProperty](http://www.w3.org/2002/07/owl#topObjectProperty)<br />
[](transferredFrom)
### transferred From
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#transferredFrom`
Description | A relation that defines that the Control of a Record has been transferred from that Role.
[](transferredTo)
### transferred To
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#transferredTo`
Description | A relation that defines that the Control of a Record has been transferred to that new Role.
[](triggeredBy)
### triggered By
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#triggeredBy`
Description | A relation that indicates that an Event has been initiated by a Trigger.
[](triggers)
### triggers
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#triggers`
Description | A relation that indicates that a Trigger has initiated a Change Event.
[](usedRecord)
### used Record
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#usedRecord`
Description | A relation between an Activity and a Record the Activity uses.
[](wasAssociatedWith)
### was Associated With
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#wasAssociatedWith`
Source | [https://www.w3.org/TR/prov-o/#wasAssociatedWith](https://www.w3.org/TR/prov-o/#wasAssociatedWith)
Description | A relation that assigns responsibility of an Agent with an Activity or Event.

## Datatype Properties
[checksum](#checksum),
[disposalClassNumber](#disposalClassNumber),
[endedAtTime](#endedAtTime),
[filename](#filename),
[filesize](#filesize),
[format](#format),
[seriesNumber](#seriesNumber),
[softwareAssignedID](#softwareAssignedID),
[startedAtTime](#startedAtTime),
[](checksum)
### checksum
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#checksum`
Description | A checksum is a small-sized datum derived from a block of digital data representing a Record for the purpose of detecting errors during the transfer or storage of a Record.
Range(s) |[xsd:float](http://www.w3.org/2001/XMLSchema#float) (c)<br />
[](disposalClassNumber)
### disposalClassNumber
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#disposalClassNumber`
Description | The number defining the sentencing requirements of a Record.
Range(s) |[xsd:integer](http://www.w3.org/2001/XMLSchema#integer) (c)<br />
[](endedAtTime)
### endedAtTime
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#endedAtTime`
Source | [https://www.w3.org/TR/prov-o/#endedAtTime](https://www.w3.org/TR/prov-o/#endedAtTime)
Description | The time at which an Activity ended.
Range(s) |[xsd:dateTime](http://www.w3.org/2001/XMLSchema#dateTime) (c)<br />
[](filename)
### filename
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#filename`
Description | A filename is a name used to uniquely identify a computer file stored in a file system.
[](filesize)
### filesize
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#filesize`
Description | File size is a measure of how much data a computer file contains or how much storage it consumes.
[](format)
### format
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#format`
Source | [http://purl.org/dc/elements/1.1/format](http://purl.org/dc/elements/1.1/format)
Description | The file format, physical medium, or dimensions of the resource.
[](seriesNumber)
### seriesNumber
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#seriesNumber`
Description | A seriesNumber is a numerical identifier for a Series.
Range(s) |[xsd:integer](http://www.w3.org/2001/XMLSchema#integer) (c)<br />
[](softwareAssignedID)
### softwareAssignedID
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#softwareAssignedID`
Description | A softwareAssignedID is an identifier given to an Artefact by an Information System.
Range(s) |[xsd:string](http://www.w3.org/2001/XMLSchema#string) (c)<br />
[](startedAtTime)
### startedAtTime
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#startedAtTime`
Source | [https://www.w3.org/TR/prov-o/#startedAtTime](https://www.w3.org/TR/prov-o/#startedAtTime)
Description | The time at which and Activity started
Range(s) |[xsd:dateTime](http://www.w3.org/2001/XMLSchema#dateTime) (c)<br />

## Annotation Properties
[contributor](#contributor),
[source](#source),
[example](#example),
[identifier](#identifier),
[name](#name),
[](contributor)
### contributor
Property | Value
--- | ---
IRI | `http://purl.org/dc/terms/contributor`
[](source)
### source
Property | Value
--- | ---
IRI | `http://purl.org/dc/terms/source`
[](example)
### example
Property | Value
--- | ---
IRI | `http://www.w3.org/2004/02/skos/core#example`
[](identifier)
### identifier
Property | Value
--- | ---
IRI | `https://schema.org/identifier`
[](name)
### name
Property | Value
--- | ---
IRI | `https://schema.org/name`

## Named Individuals
[Active](#Active),
[Approved](#Approved),
[AwaitingDisposal](#AwaitingDisposal),
[Completed](#Completed),
[Confidential](#Confidential),
[Disapproved](#Disapproved),
[Disposed](#Disposed),
[Highly Protected](#HighlyProtected),
[Protected](#Protected),
[Redundant](#Redundant),
[RetainAsNationalArchives](#RetainAsNationalArchives),
[Secret](#Secret),
[Top Secret (NV)](#TopSecret(NV)),
[Top Secret (PV)](#TopSecret(PV)),
[Unclassified](#Unclassified),
### Active <sup>c</sup>
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#Active`
* **Contributor(s)**
  * [Status](http://linked.data.gov.au/def/agrif#Status)
### Approved <sup>c</sup>
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#Approved`
* **Contributor(s)**
  * [DecisionStatus](http://linked.data.gov.au/def/agrif#DecisionStatus)
### AwaitingDisposal <sup>c</sup>
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#AwaitingDisposal`
* **Contributor(s)**
  * [Status](http://linked.data.gov.au/def/agrif#Status)
### Completed <sup>c</sup>
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#Completed`
* **Contributor(s)**
  * [Status](http://linked.data.gov.au/def/agrif#Status)
### Confidential <sup>c</sup>
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#Confidential`
* **Contributor(s)**
  * [SecurityClassification](http://linked.data.gov.au/def/agrif#SecurityClassification)
### Disapproved <sup>c</sup>
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#Disapproved`
* **Contributor(s)**
  * [DecisionStatus](http://linked.data.gov.au/def/agrif#DecisionStatus)
### Disposed <sup>c</sup>
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#Disposed`
* **Contributor(s)**
  * [Status](http://linked.data.gov.au/def/agrif#Status)
### Highly Protected <sup>c</sup>
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#HighlyProtected`
* **Contributor(s)**
  * [SecurityClassification](http://linked.data.gov.au/def/agrif#SecurityClassification)
### Protected <sup>c</sup>
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#Protected`
* **Contributor(s)**
  * [SecurityClassification](http://linked.data.gov.au/def/agrif#SecurityClassification)
### Redundant <sup>c</sup>
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#Redundant`
* **Contributor(s)**
  * [Status](http://linked.data.gov.au/def/agrif#Status)
### RetainAsNationalArchives <sup>c</sup>
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#RetainAsNationalArchives`
* **Contributor(s)**
  * [DisposalClass](http://linked.data.gov.au/def/agrif#DisposalClass)
### Secret <sup>c</sup>
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#Secret`
* **Contributor(s)**
  * [SecurityClassification](http://linked.data.gov.au/def/agrif#SecurityClassification)
### Top Secret (NV) <sup>c</sup>
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#TopSecretNV`
* **Contributor(s)**
  * [SecurityClassification](http://linked.data.gov.au/def/agrif#SecurityClassification)
### Top Secret (PV) <sup>c</sup>
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#TopSecretPV`
* **Contributor(s)**
  * [SecurityClassification](http://linked.data.gov.au/def/agrif#SecurityClassification)
### Unclassified <sup>c</sup>
Property | Value
--- | ---
IRI | `http://linked.data.gov.au/def/agrif#Unclassified`
* **Contributor(s)**
  * [SecurityClassification](http://linked.data.gov.au/def/agrif#SecurityClassification)
## Namespaces
* **default (:)**
  * `http://linked.data.gov.au/def/agrif#`
* **:**
  * `http://linked.data.gov.au/def/agrif#`
* **dcterms**
  * `http://purl.org/dc/terms/`
* **owl**
  * `http://www.w3.org/2002/07/owl#`
* **prov**
  * `http://www.w3.org/ns/prov#`
* **rdf**
  * `http://www.w3.org/1999/02/22-rdf-syntax-ns#`
* **rdfs**
  * `http://www.w3.org/2000/01/rdf-schema#`
* **sdo**
  * `https://schema.org/`
* **skos**
  * `http://www.w3.org/2004/02/skos/core#`
* **vann**
  * `http://purl.org/vocab/vann/`
* **xml**
  * `http://www.w3.org/XML/1998/namespace`
* **xsd**
  * `http://www.w3.org/2001/XMLSchema#`

## Legend
* Classes: c
* Object Properties: op
* Functional Properties: fp
* Data Properties: dp
* Annotation Properties: dp
* Properties: p
* Named Individuals: ni