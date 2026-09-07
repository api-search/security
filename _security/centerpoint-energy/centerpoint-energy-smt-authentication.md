---
anonymous_access: false
api_key_in: []
auth_types: []
description: Two-factor transport plus credential authentication. Every API call is made over mutual TLS with a signed, registered API SSL certificate whose domain name must match the requesting entity, and carries an HTTP Basic authorization header with an ID/password pair created by the entity account owner in the SMT 3.0 portal. Credentials are scoped per DUNS number; a service provider representing multiple entities needs a separate unique SSL certificate per entity. Wildcard certificates are rejected.
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Centerpoint Energy Smt Authentication
name_suffix: Authentication
oauth_flows: []
overview: CenterPoint Energy declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: CenterPoint Energy
provider_slug: centerpoint-energy
scheme_count: 0
schemes: []
slug: centerpoint-energy-smt-authentication
source_filename: centerpoint-energy-smt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: CenterPoint Energy\nproviderId: centerpoint-energy\napi: centerpoint-energy:usage-history-inquiry\ngenerated: '2026-09-05'\nmethod: searched\nsource: https://www.smartmetertexas.com/commonapi/gethelpguide/help-guides/Smart_Meter_Texas_Interface_Guide.pdf\ndocs: https://www.smartmetertexas.com/commonapi/gethelpguide/help-guides/Smart_Meter_Texas_Interface_Guide.pdf\nnote: >-\n  Read from section 2 (Security Integration Requirements) of the Smart Meter Texas 3.0 Data Access\n  Interface Guide dated February 26, 2024, fetched at HTTP 200. Smart Meter Texas is jointly owned and\n  funded by the four Texas TDSPs including CenterPoint Energy Houston Electric, and is the interface\n  CenterPoint's competitive-retailer documentation directs third parties to for CenterPoint meter data;\n  the auth scheme below is SMT's, and applies to every CenterPoint ESI ID reached through it. No\n  OpenAPI securitySchemes\
  \ block exists to derive from — SMT publishes no machine-readable contract.\ndescription: >-\n  Two-factor transport plus credential authentication. Every API call is made over mutual TLS with a\n  signed, registered API SSL certificate whose domain name must match the requesting entity, and carries\n  an HTTP Basic authorization header with an ID/password pair created by the entity account owner in the\n  SMT 3.0 portal. Credentials are scoped per DUNS number; a service provider representing multiple\n  entities needs a separate unique SSL certificate per entity. Wildcard certificates are rejected.\nsecuritySchemes:\n  - id: smt_mutual_tls\n    type: mutualTLS\n    description: >-\n      Signed registered API SSL certificate required per SMT entity account. The production certificate's\n      domain name must match the entity domain name; unsigned certificates are accepted for testing only;\n      no wildcard certificates are accepted. Third-party service providers need one unique certificate\
  \ per\n      entity they represent.\n    required: true\n  - id: smt_http_basic\n    type: http\n    scheme: basic\n    description: >-\n      One set of API credentials (ID and password) per DUNS associated with an SMT account, created by the\n      entity account owner in the SMT 3.0 portal. A missing header returns 403\n      {\"error\":\"Basic authentication header is missing.\"}; a wrong pair returns 401\n      {\"error\":\"Incorrect username or password.\"}.\n    required: true\n  - id: smt_requester_identity\n    type: payloadField\n    description: >-\n      Beyond transport and credential auth, each request body carries requesterID, requesterType and\n      requesterAuthenticationID fields identifying the acting entity, and data access for a given ESI ID\n      is additionally gated by an executed Energy Data Sharing Agreement between the customer and the\n      requesting party.\n    required: true\ntransport:\n  tls_versions_supported:\n    - TLSv1.0\n    - TLSv1.1\n    - TLSv1.2\n\
  \  mutual_tls: true\n  note: >-\n    The guide states only TLS 1.0-1.2 are supported for the integration channel and that mutual TLS\n    authentication is required. TLS 1.0/1.1 are deprecated protocols; recorded here verbatim as published,\n    not endorsed.\noauth2: false\napi_keys: false\nopenid_connect: false\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centerpoint-energy/refs/heads/main/authentication/centerpoint-energy-smt-authentication.yml
summary_line: 0 schemes
tags:
- EDI
- ERCOT
- Electricity
- Energy
- Fortune 500
- Green Button
- Interval Data
- NAESB ESPI
- Natural Gas
- Smart Meter
- Texas
- TxSET
- Usage Data
- Utility
---
