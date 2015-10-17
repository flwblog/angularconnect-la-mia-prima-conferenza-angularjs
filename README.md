# angularconnect-la-mia-prima-conferenza-angularjs

<img src="https://cloud.githubusercontent.com/assets/949194/10559801/92414b0a-74f8-11e5-89e3-75509c676ef0.jpg" style="width: 80%"/>

This document contains the definitions and terms that are common between the **Business Document
Exchange Network (BUSDOX) service metadata** and transport specifications. 

These are:

* **The START** and **LIME** transport specifications
* The **SML (Service Metadata Locator)** and **SMP (Service Metadata Publishing)** specifications
* A scheme for process identifiers.

The set of peer Access Points and Service Metadata Publishing and Locator services that:

1. Meet the governance requirements of any BUSDOX infrastructure instance
2. Are listed as endpoints by BUSDOX Service Metadata Publishers
3. Are accessible under service level agreements for APs defined in any instance of a BUSDOX
infrastructure


## BUSDOX Infrastructure


**Access Point/AP**: a peer in a BUSDOX Infrastructure instance.  
* Source Access Point (SrcAP): an Access Point sending a message to another Access Point
* Destination Access Point (DestAP): an Access Point receiving a message from a SrcAP.

**SAML Token/Assertion**: The terms SAML token and SAML assertion will be used interchangeably.

**Secure Trusted Asynchronous Reliable Transport (START)**: The Secure Trusted Asynchronous Reliable
Transport, see the START transport specification.

**Lightweight Message Exchange/LIME**: The Lightweight Message Exchange Transport, see the LIME transport
specification.

**Lightweight Client/LC**: Client application that communicates with a LIME compliant Access Point
(LIME-AP)

**Lightweight Profile Access Point/LIME-AP**: A BUSDOX Access Point that exposes the Lightweight
Profile Interface towards client applications. An LIME-AP may be an existing VAN or a new service
offered by governments or private companies.

**Message Channel/M**C: An LIME-AP offers a Message Channel (MC) interface to the LC. There are
(at least) two MCs available to the LC.

**Inbound/Outbound Message Channel/InMC/OutMC**: An Inbound Message Channel stores messages
destined for the LC, and the Outbound Message Channel is used by the LC as a relay for messages
destined for other companies.

**Endpoint Reference/EPR**: Each Message Channel of a LIME-AP is uniquely identified by a WSAddressing
Endpoint Reference (EPR)

**Channel Identifier/ChannelID**: A channel of an LIME-AP.

**Service Metadata Locator service/SML**: A service which provides a client with the capability of
discovering the **Service Metadata Publisher endpoint** associated with a particular participant
identifier.  
A client uses this service in order to find where information is held about services for a
particular participant business.

**Service Metadata Publisher/SMP**: A service metadata publisher offers a service on the network
where information about services of specific participant businesses can be found and retrieved.   
It is necessary for a client application to retrieve the metadata about the services for a target participant
business before the client can use those services to send messages to the participant business.

**Service Metadata Consumer/SMC**: A Service Metadata Consumer is any entity consuming Service
Metadata provided by a Service Metadata Publisher. This is typically the sender of the document, or
the sender side Access Point.

**Participant Identifier**: A participant business level identifier such as **GLN** (a GS1 Global Location
Number) or **DUNS** (Dun & Bradstreet) number that is used to identify a trading partner.  
In the context of BUSDOX, participant identifiers are used to discover services associated with trading
partners in Service Metadata.

**Secure Token Service/STS**: a service that offers security tokens to network clients.

**Transport Layer Security/TLS**: Transport Layer Security is the standard most used to secure HTTP. It is the
successor to Secure Sockets Layer (SSL).

**Service Metadata Publisher Certificate** (SMP Certificate): A certificate used by a specific SMP to create all
signatures of the signed resources. 



## References

[PEPPOL Transport Infrastructure BusDox Common  Definitions](https://joinup.ec.europa.eu/svn/peppol/PEPPOL_EIA/1-ICT_Architecture/1-ICT-Transport_Infrastructure/13-ICT-Models/ICT-Transport-BusDox_Definitions-101.pdf)
