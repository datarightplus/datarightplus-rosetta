%%%

title = "DataRight+ Rosetta Stone"
area = "Internet"
workgroup = "datarightplus-parity"
submissionType = "independent"

[seriesInfo]
name = "Internet-Draft"
value = "draft-authors-datarightplus-rosetta-latest"
stream = "independent"
status = "informational"

date = 2024-03-28T00:00:00Z

[[author]]
initials="S."
surname="Low"
fullname="Stuart Low"
organization="Biza.io"
[author.address]
email = "stuart@biza.io"

[[author]]
initials="B."
surname="Kolera"
fullname="Ben Kolera"
organization="Biza.io"
[author.address]
email = "bkolera@biza.io"

%%%

.# Abstract

A rosetta stone for the DataRight Plus specifications.

{mainmatter}

# Scope

The scope of this document is limited to the conversion of terms utilised within the DataRight Plus specification suite to jurisdictional terms within legal frameworks. The intent of delivering this document is to remove ambiguity from the broader specification set by isolating, generally legal, terms within a single document.

# Terminology

This document defines the following terms:

Certificate Practice Statement
: A statement of the practices that a certification authority (CA) employs in issuing, suspending, revoking, and renewing certificates and providing access to them, in accordance with specific requirements.

CDR
:  Consumer Data Right

CDR Sharing Arrangement
: A legal construct, established by the [@!CDR-RULES] representing a disclosure consent between a Provider and a Initiator via a Software Product.

CDR Sharing Arrangement Identifier
: A unique and persistent identifier, typically a UUID or similar, that represents a reference to a CDR Sharing Arrangement.

Consumer
: A Consumer represents an individual or an entity for which a User has been granted permissions to perform actions on behalf of.

Data Set Language
: When requesting consent to conduct actions a Provider must present a description of the action or data being permitted. The Data Set Language is a prescription of what this text **MUST** be.

Ecosystem Authority
: The Ecosystem Authority represents the designated arbiter of trust between Providers, Initiators and the Consumer. Further elaboration on the Ecosystem Authority is provided within [@!DATARIGHTPLUS-ADMISSION-CONTROL].

Electricity Authority
: The Electricity Authority represents the holder of information pertaining to electricity meters and usage.

Electricity Plan Website
: The Electricity Plan Website represents the holder of information pertaining to electricity plan information

Initiator
: A Initiator is a client application which conducts activities with a Provider server. In an authorisation context a Initiator is analogous with an [@!OIDC-Core] Relying Party (RP).

Initiator Arrangement Revocation Endpoint (ICARE)
: A specific URI for the purposes of issuing ICARE requests as described in [@!DATARIGHTPLUS-SHARING-ARRANGEMENT-V1-00].

Initiator Base URI (IBU)
: The Base URI used for all calls to Initiator hosted resource server endpoints.

Personally Identifiable Information (PII)
: Information that (a) can be used to identify the natural person to whom such information relates, or (b) is or might be directly or indirectly linked to a natural person to whom such information relates.

Provider
: A Provider is a piece of server infrastructure which receives requests from an Initiator. In an authorisation context a Provider is analogous with an [@!OIDC-Core] OpenID Provider (OP).

User
: A User is a human who provides an identifier unique to the individual and for which correlates to one or more Consumer relationships. In an authorisation context a User is analogous with an [@!OIDC-Core] End-User.

# Ecosystem Specific Mappings

The following table provides a mapping from DataRight+ terminology to ecosystem specific terms.

| DataRight+            | Australian CDR              |
|-----------------------|-----------------------------|
| Electricity Authority | AEMO                        |
| Initiator             | Software Product            |
| Initiator Brand       | Data Recipient Brand        |
| Initiator Entity      | Data Recipient Legal Entity |
| Initiator Base URI    | Recipient Base URI          |
| Provider              | Data Holder Brand           |
| Provider ID           | Data Holder Brand ID        |
| Provider Entity       | Data Holder                 |
| Consumer              | CDR Consumer                |
| Ecosystem Directory   | CDR Register                |
| Ecosystem Authority   | ACCC                        |
| User                  | User                        |
| User Agent            | User Agent                  |

## Australian Consumer Data Right

### CDR Consumer

A CDR Consumer is a business or individual who authorises the sharing of data stored by a CDR Data Holder on their behalf to a CDR Software Product with their permission. A User, regardless of their individual relationship with a Data Holder may also have access to zero or more non-individual Consumer's, for instance businesses that they have permission to make decisions for.

It is critical to note that a CDR Consumer is the individual entity of which data is being shared or actions are being performed on. Within the CDR there are various relationship types including:

- Nominated Representatives: Authorised representatives of a specific corporate entity, for instance a company director
- Secondary Users: Authorised parties who can access an individual Consumers data

### Data Holder Brand
For the purposes of this specification a Data Holder is described as the party who is offering or has offered services to the Consumer and/or holds relevant data related to those services on behalf of the Consumer.

The types and format of that data is outside the scope of this particular specification but traditionally includes:

- specific customer information such as name, addresses and phone numbers;
- information related to services such as account numbers, pricing information and balances;
- transaction/ledger information pertaining to services provided

Within the CDR ecosystem the mandated Data Holders are ostensible Banking and Energy providers. Additional sectors can be designated by way of a legally binding Designation Instrument coupled with changes to the CDR Rules.

### Legal Entity


### Data Recipient

A CDR Data Recipient is a party that provides activities, such as data sharing, through the Consumer who participates in the authorisation process initiated by a Initiator. Please refer to the expanded description of Provider within this document.

### Software Product

A Software Product is the listed value proposition, provided by a Data Recipient, which accesses a Data Holder Brand.

### CDR Register

# Acknowledgement

The following people contributed to this document:

- Stuart Low (Biza.io) - Editor
- Ben Kolera (Biza.io)

{backmatter}

<reference anchor="CDR Rules" target="https://www.legislation.gov.au/F2020L00094"> <front> <title>Competition and Consumer (Consumer Data Right) Rules 2020</title> <author initials="Australian" surname="Treasury" fullname="Australian Treasury"> <organization>Australian Government</organization> </author><date day="22" month="Jul" year="2023"/> </front> </reference>

<reference anchor="OIDC-Core" target="http://openid.net/specs/openid-connect-core-1_0.html"> <front> <title>OpenID Connect Core 1.0 incorporating errata set 1</title> <author initials="N." surname="Sakimura" fullname="Nat Sakimura"> <organization>NRI</organization> </author> <author initials="J." surname="Bradley" fullname="John Bradley"> <organization>Ping Identity</organization> </author> <author initials="M." surname="Jones" fullname="Mike Jones"> <organization>Microsoft</organization> </author> <author initials="B." surname="de Medeiros" fullname="Breno de Medeiros"> <organization>Google</organization> </author> <author initials="C." surname="Mortimore" fullname="Chuck Mortimore"> <organization>Salesforce</organization> </author> <date day="8" month="Nov" year="2014"/> </front> </reference>

<reference anchor="DATARIGHTPLUS-ADMISSION-CONTROL" target="https://datarightplus.github.io/datarightplus-admission-control/draft-datarightplus-admission-control.html"> <front><title>DataRight+ Admission Control: Baseline</title><author initials="S." surname="Low" fullname="Stuart Low"><organization>Biza.io</organization></author></front> </reference>






