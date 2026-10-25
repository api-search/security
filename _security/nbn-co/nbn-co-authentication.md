---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Nbn Co Authentication
name_suffix: Authentication
oauth_flows: []
overview: NBN Co declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: NBN Co
provider_slug: nbn-co
scheme_count: 2
schemes:
- description: Digital certificates created by nbn from information the RSP supplies, used in connection with B2B Access.
  evidence: provide to nbn all information reasonably required and requested by nbn to create any digital certificates and security protocols to be used in connection with B2B Access
  name: digital-certificates
  note: The terms say "digital certificates"; that this is mutual TLS is an inference from that wording, not stated.
  type: mutualTLS
  type_confidence: low
- description: API Credentials issued by nbn to the RSP for B2B Access via the nbn-hosted API gateway; treated as nbn Confidential Information.
  evidence: manage digital certificates and API Credentials as Confidential Information of nbn
  name: api-credentials
  type: unspecified
slug: nbn-co-authentication
source_filename: nbn-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: NBN Co authentication\ngenerated: '2026-10-22'\nmethod: searched\nsource: https://www.nbnco.com.au/content/dam/nbn/documents/sell/wba/2024/sfaa-wba-nbn-platform-interfacing-service-service-terms-20241003.pdf.coredownload.pdf\ndocs: https://www.nbnco.com.au/content/dam/nbn/documents/sell/wba/2024/sfaa-wba-nbn-platform-interfacing-service-service-terms-20241003.pdf.coredownload.pdf\nnote: >-\n  No public API or OpenAPI is published. The WBA nbn Platform Interfacing Service service terms\n  (HTTP 200, application/pdf, fetched 2026-10-22) describe B2B Access through an API gateway hosted\n  by nbn secured with digital certificates and API Credentials issued to contracted retail service\n  providers (RSPs). The B2B Specifications that define the actual security protocols are confidential\n  and were not read; scheme details below are only what the terms state.\nschemes:\n- name: digital-certificates\n  type: mutualTLS\n  type_confidence: low\n  description: Digital certificates\
  \ created by nbn from information the RSP supplies, used in connection with B2B Access.\n  evidence: \"provide to nbn all information reasonably required and requested by nbn to create any digital certificates and security protocols to be used in connection with B2B Access\"\n  note: The terms say \"digital certificates\"; that this is mutual TLS is an inference from that wording, not stated.\n- name: api-credentials\n  type: unspecified\n  description: API Credentials issued by nbn to the RSP for B2B Access via the nbn-hosted API gateway; treated as nbn Confidential Information.\n  evidence: \"manage digital certificates and API Credentials as Confidential Information of nbn\"\naccess:\n  audience: contracted retail service providers under the Wholesale Broadband Agreement\n  developer_portal: \"nbn® Developer Portal (access information supplied to RSPs; confidential, no public URL)\"\n  evidence: \"acquire access information in relation to the nbn® Developer Portal and maintain such\
  \ access information as Confidential Information of nbn\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nbn-co/refs/heads/main/authentication/nbn-co-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Telecommunications
- Broadband
- Wholesale
- Australia
- Network Infrastructure
- B2B
---
