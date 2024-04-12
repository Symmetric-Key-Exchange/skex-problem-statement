---
title: "Symmetric Key Exchange Problem Statement"
abbrev: "TODO - Abbreviation"
category: info

docname: draft-aelmans-skex-problem-statement-latest
submissiontype: IETF
number:
date:
consensus: true
v: 3
# area: SEC
# workgroup: SKEX
keyword:
 - next generation
 - unicorn
 - sparkling distributed ledger
venue:
#  group: WG
#  type: Working Group
#  mail: skex@ietf.org
#  arch: https://example.com/WG
  github: "Symmetric-Key-Exchange/skex-problem-statement"
  latest: "https://Symmetric-Key-Exchange.github.io/skex-problem-statement/draft-aelmans-skex-problem-statement.html"

author:
 -
    fullname: Melchior Aelmans
    organization: Juniper Networks
    email: melchior@juniper.net

normative:

informative:


--- abstract

Asymmetric cryptography and Public-key cryptography mechanisms are considered to be vulnerable to quantum computer attacks, posing a challenge to data security and integrity. Furthermore, there are use cases where asymmetric cryptography is not a good fit to solve the problem of key distribution, examples include computationally constrained devices. This document outlines and describes the challenges with currently widely used Asymmetric cryptography and Public-key cryptography.


--- middle

# Introduction

The current context presents challenges for communication security on the Internet:
* Asymmetric-key cryptography is a versatile tool for securing communication but it does have some shortcomings and limitations, including that:
 - It is generally computationally intensive
 - Its security relies on the complexity of solving mathematical problems
 - The arrival of the quantum era is now additionally jeopardizing the security of key exchanges based on asymmetric cryptography.
* Post Quantum Cryptography (PQC) algorithms show some promise against quantum attacks, but are unproven and * typically computationally intensive and require increased message sizes.
* Quantum Key Distribution (QKD) has desirable properties, but is unsuitable for general use on the internet.
* Symmetric key cryptography is well-trusted, including Pre-Shared keys (PSK), though the key distribution presents a challenge.

This leads to the need to address the problem of symmetric key establishment and standardization:
* Symmetric key distribution mechanisms and protocols are not yet standardized.
* Several government institutions and users of cryptography have requested newer and standardized methods for symmetric key distribution mechanisms.
* System integrators and architects need to be able to abstract the symmetric key distribution so that their systems do not depend on a specific vendor.
* Existing interface standards do not address all abstraction levels nor the range of applications. For example, ETSI GS QKD 014 is a high-level protocol, unsuited to internal low-level APIs.
* Security of key management must be considered in a wide range of contexts.
* Systems that may be deployed widely must be highly scalable.


# Conventions and Definitions

{::boilerplate bcp14-tagged}


# Security Considerations

TODO Security


# IANA Considerations

This document has no IANA actions.


--- back

# Acknowledgments
{:numbered="false"}

TODO acknowledge.
