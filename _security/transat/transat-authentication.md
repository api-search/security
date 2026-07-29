---
api_key_in: []
auth_types:
- vendor-credential-exchange
description: 'Air Transat''s direct-connect distribution API does not use OAuth, OpenID Connect, API keys or mutual TLS. It uses a two-stage vendor credential exchange inherited from the Radixx (Sabre) passenger service system: a system-level logon that returns a session GUID, followed by a travel-agent logon that binds that session to a Transat-assigned IATA agency. There is no self-serve key issuance, no developer portal and no sandbox; every credential is provisioned by Transat under a commercial agreement.'
kind: authentication
layout: security
method: searched
name: Transat Authentication
name_suffix: Authentication
oauth_flows: []
overview: Transat secures its APIs with vendor-credential-exchange across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Transat
provider_slug: transat
scheme_count: 2
schemes:
- credentials:
  - AccessibleCarrierCode
  - LogonID
  - Password
  description: System-level authentication. Exchanges a Transat-issued Radixx LogonID and Password, scoped to AccessibleCarrierCode "TS", for a SecurityGUID that scopes the remainder of the booking flow.
  name: RetrieveSecurityToken
  returns: SecurityGUID
  stage: 1
  transport: SOAP 1.1
  type: vendor-credential-exchange
- credentials:
  - SecurityGUID
  - AccessibleCarrierCode
  - IATANumber
  - UserName
  - Password
  description: 'Agency-level authentication. Binds the session to a pre-defined travel agency that Transat configures for each partner. The specification states: "A pre-defined Travel Agency will be configured and provided to each OTA Partner."'
  name: LoginTravelAgent
  stage: 2
  transport: SOAP 1.1
  type: vendor-credential-exchange
slug: transat-authentication
source_filename: transat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: searched\nsource: >-\n  https://staticcontent.transat.com/airtransat/pdf/EN/NDC-TS-Radixx-ConnectPoint-API-book-Flight.pdf\n  — \"Air Transat API specifications\", Radixx ConnectPoint API, Flight Booking\n  Detailed View, v2.2.4 (May 2023), the only technical contract Air Transat\n  publishes. Cross-checked against review.yml (probed 2026-07-28).\ndocs: https://www.airtransat.com/en-CA/air-transat-ndc\ndescription: >-\n  Air Transat's direct-connect distribution API does not use OAuth, OpenID\n  Connect, API keys or mutual TLS. It uses a two-stage vendor credential\n  exchange inherited from the Radixx (Sabre) passenger service system: a\n  system-level logon that returns a session GUID, followed by a travel-agent\n  logon that binds that session to a Transat-assigned IATA agency. There is no\n  self-serve key issuance, no developer portal and no sandbox; every credential\n  is provisioned by Transat under a commercial agreement.\n\nsummary:\n\
  \  types: [vendor-credential-exchange]\n  standards: []\n  oauth2: false\n  openid_connect: false\n  api_key: false\n  mutual_tls: not published\n  self_serve: false\n  spec_format: SOAP 1.1 / .NET WCF (no WSDL published)\n\nschemes:\n- name: RetrieveSecurityToken\n  type: vendor-credential-exchange\n  stage: 1\n  transport: SOAP 1.1\n  credentials:\n  - AccessibleCarrierCode  # fixed value \"TS\"\n  - LogonID                # Radixx system logon issued by Transat\n  - Password\n  returns: SecurityGUID\n  description: >-\n    System-level authentication. Exchanges a Transat-issued Radixx LogonID and\n    Password, scoped to AccessibleCarrierCode \"TS\", for a SecurityGUID that\n    scopes the remainder of the booking flow.\n- name: LoginTravelAgent\n  type: vendor-credential-exchange\n  stage: 2\n  transport: SOAP 1.1\n  credentials:\n  - SecurityGUID           # from RetrieveSecurityToken\n  - AccessibleCarrierCode\n  - IATANumber             # must be \"Active in RADIXX\"\n  - UserName\
  \               # agency user issued by Transat\n  - Password\n  description: >-\n    Agency-level authentication. Binds the session to a pre-defined travel\n    agency that Transat configures for each partner. The specification states:\n    \"A pre-defined Travel Agency will be configured and provided to each OTA\n    Partner.\"\n\nsession:\n  token: SecurityGUID\n  lifetime: not published\n  renewal: >-\n    The session is closed after SavePNR at the end of the main booking flow;\n    RetrieveSecurityToken must be called again for subsequent work such as\n    retrieving a PNR.\n  refresh_token: none\n  revocation: not published\n\nscopes:\n  model: none\n  note: >-\n    No scope, permission or consent surface is published. Authorization is\n    carrier-scoped (AccessibleCarrierCode \"TS\") and agency-scoped (IATANumber),\n    both assigned by Transat, not requested by the client.\n  artifact: null   # scopes/ intentionally absent — this is not an OAuth provider\n\nprovisioning:\n  self_serve:\
  \ false\n  gate: commercial-agreement\n  contact: commercial.ndc@transat.com\n  steps:\n  - Contact Air Transat commercial / NDC connectivity and enter a partner agreement.\n  - Transat configures a pre-defined travel agency in Radixx for the partner.\n  - Transat issues a Radixx LogonID + Password for RetrieveSecurityToken.\n  - Transat issues an IATA number that must be Active in RADIXX.\n  - Transat issues an agency UserName + Password for LoginTravelAgent.\n  sandbox: none published\n  trial: none published\n\ntransport_security:\n  published_base_url: false\n  note: >-\n    No endpoint host, WSDL location or sandbox URL appears anywhere in the\n    46-page specification. The service address is supplied privately to each\n    partner, so transport security cannot be verified from public sources.\n    See security/transat-domain-security.yml for the public web hosts.\n\nrelated:\n  conventions: conventions/transat-conventions.yml\n  conformance: conformance/transat-conformance.yml\n\
  \  lifecycle: lifecycle/transat-lifecycle.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transat/refs/heads/main/authentication/transat-authentication.yml
summary_line: vendor-credential-exchange · 2 schemes
tags:
- Travel
- Canada
- Aviation
- Airline
- Distribution
- NDC
- Booking
- Tour Operator
- Corporate Travel
- GDS
---
