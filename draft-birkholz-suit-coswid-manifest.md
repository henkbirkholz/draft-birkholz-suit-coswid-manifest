---
title: A SUIT Manifest Extension for Concise Software Identifiers 
abbrev: CoSWID SUIT Extension
docname: draft-birkholz-suit-coswid-manifest-latest
stand_alone: true
ipr: trust200902
area: Security
wg: SUIT Working Group
kw: Internet-Draft
cat: std
pi:
  toc: yes
  sortrefs: yes
  symrefs: yes

author:
- ins: H. Birkholz
  name: Henk Birkholz
  org: Fraunhofer SIT
  abbrev: Fraunhofer SIT
  email: henk.birkholz@sit.fraunhofer.de
  street: Rheinstrasse 75
  code: '64295'
  city: Darmstadt
  country: Germany

normative:
  RFC2119:
  I-D.ietf-sacm-coswid: COSWID
  I-D.ietf-suit-information-model: SUITIM
  I-D.ietf-suit-architecture: SUITARCH

--- abstract

This document defines a resource extension for Concise Software Identifiers (CoSWID) that represents a SUIT firmware manifest. This extension combines the information elements of the SUIT information model with the semantic expressiveness of Software Identifiers. In consequence, this composite enables the integration of Firmware Updates for the Internet of Things (SUIT) in existing work-flows for updates of software components in general.

--- middle

# Introduction

Firmware updates are quite similar to a software update of applications -- composites of software components -- for example, servers or user-devices. The attributes and semantic dependencies as defined by Concise Software Identifies {{-COSWID}} are equivalent. In contrast, location and target definitions as well as the characteristics that are specific to an update campaign of a SUIT require a specific set of addiction information. The semantics regarding SUIT specific information elements are defined by the SUIT Information Model {{-SUITIM}}. Correspondingly, the CoSWID extension defined in this document uses CDDL extension points to add SUIT information elements to the standard Concise Software Identifiers.

# SUIT Manifest Extension

The following CDDL data definition is intended to be used as an extension to the CoSWID CDDL data definition. Corresponding terms, such as Resources, Processors and Targets of input nodes and output nodes are covered by the SUIT Information Model and Architecture {{-SUITARCH}}.

# SUIT Manifest Resource Data Definition

The following CDDL can be added to Payload or Evidence Resources as defined by Concise Software Identifiers.

~~~ CDDL
{::include suit-manifest-resource.cddl}
~~~

# Future Updates

This draft is intended to incorporate the extension registry that will be defined by Concise Software Identifiers. Until then, a consecutive numbering system in alignment to the labels used in Concise Software Identifiers is used.

#  Security Considerations

TBD

#  Acknowledgments

TBD

#  Change Log

Initial Contribution

# Contributors

TBD

--- back
