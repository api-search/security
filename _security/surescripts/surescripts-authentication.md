---
api_key_in:
- header
auth_types:
- mutualTLS
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Surescripts Authentication
name_suffix: Authentication
oauth_flows: []
overview: Surescripts secures its APIs with mutualTLS and apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Surescripts
provider_slug: surescripts
scheme_count: 4
schemes:
- description: Client certificate issued by the Surescripts Certification Authority, presented on every request. Surescripts validates the certificate and resolves it to an Account ID and Participant ID, which determine product entitlement and data access.
  evidence:
  - 'Formulary Download API: "restricts content based on the account of the user accessing the system - identified by the MTLS client certificate submitted in the request"'
  - 'Medication History for Populations: "For authentication, requests will use mTLS where the client will provide a client certificate"'
  - 'Live probe 2026-08-15: care-coordination.surescripts.net presents a leaf cert issued by "Surescripts Issuing Certification Authority" chaining to "Surescripts Root Certification Authority"; an anonymous request is reset before any HTTP response.'
  issued_by: Surescripts Issuing Certification Authority
  name: mutualTLS
  obtained_via: Surescripts onboarding / certification process
  self_serve: false
  sources:
  - https://docs.surescripts.com/formulary-download/guide/security-and-data-access
  - https://docs.surescripts.com/medhistory-populations/guide/integration-and-production
  type: mutualTLS
- applies_to: Formulary Download API
  description: Participant ID of the requesting organization. Used together with the mTLS client certificate to determine the NCPDP Formulary & Benefit version(s) available, the preferred drug database, and per-file permission restrictions.
  in: header
  name: x-participant-id
  parameter_name: x-participant-id
  required: true
  sources:
  - https://docs.surescripts.com/formulary-download/guide/api-details
  - https://docs.surescripts.com/formulary-download/guide/security-and-data-access
  type: apiKey
- applies_to: Medication History for Populations FHIR API
  description: Participant ID of the sender, e.g. T00000000012345 (the leading T denotes a staging / test participant). Accompanied by the mandatory X-SENDER-UID-QUALIFIER header, fixed value 10.
  in: header
  name: X-SENDER-UID
  parameter_name: X-SENDER-UID
  required: true
  sources:
  - https://docs.surescripts.com/medhistory-populations/guide/http-request-headers
  type: apiKey
- applies_to: Medication History for Populations FHIR API
  fixed_value: '10'
  in: header
  name: X-SENDER-UID-QUALIFIER
  parameter_name: X-SENDER-UID-QUALIFIER
  required: true
  sources:
  - https://docs.surescripts.com/medhistory-populations/guide/http-request-headers
  type: apiKey
slug: surescripts-authentication
source_filename: surescripts-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: searched\nsource: https://docs.surescripts.com/formulary-download/guide/security-and-data-access\ndocs:\n  - https://docs.surescripts.com/formulary-download/guide/security-and-data-access\n  - https://docs.surescripts.com/medhistory-populations/guide/http-request-headers\n  - https://docs.surescripts.com/medhistory-populations/guide/integration-and-production\n  - https://docs.surescripts.com/connectivity/home\n  - https://surescripts.com/why-surescripts/certifications-and-accreditations\nnote: >-\n  Derived by reading the public pages of the Surescripts Developer Portal\n  (docs.surescripts.com), not from an OpenAPI - Surescripts publishes no machine-readable\n  contract. Surescripts does not use OAuth, OIDC or bearer API keys anywhere in its public\n  documentation. Every documented API surface authenticates the CALLING ORGANIZATION with a\n  Surescripts-issued client certificate over mutual TLS, then authorizes the request with a\n  Participant\
  \ ID carried in an HTTP header. Surescripts operates its own Certificate\n  Authority and Registration Authority (see the Surescripts Certification Practice Statement\n  on the certifications page), which is why its API hosts present a private-root chain.\nsummary:\n  types:\n    - mutualTLS\n    - apiKey\n  api_key_in:\n    - header\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  bearer_tokens: false\n  self_serve_credentials: false\nschemes:\n  - name: mutualTLS\n    type: mutualTLS\n    description: >-\n      Client certificate issued by the Surescripts Certification Authority, presented on\n      every request. Surescripts validates the certificate and resolves it to an Account ID\n      and Participant ID, which determine product entitlement and data access.\n    issued_by: Surescripts Issuing Certification Authority\n    self_serve: false\n    obtained_via: Surescripts onboarding / certification process\n    sources:\n      - https://docs.surescripts.com/formulary-download/guide/security-and-data-access\n\
  \      - https://docs.surescripts.com/medhistory-populations/guide/integration-and-production\n    evidence:\n      - >-\n        Formulary Download API: \"restricts content based on the account of the user accessing\n        the system - identified by the MTLS client certificate submitted in the request\"\n      - >-\n        Medication History for Populations: \"For authentication, requests will use mTLS where\n        the client will provide a client certificate\"\n      - >-\n        Live probe 2026-08-15: care-coordination.surescripts.net presents a leaf cert issued by\n        \"Surescripts Issuing Certification Authority\" chaining to \"Surescripts Root Certification\n        Authority\"; an anonymous request is reset before any HTTP response.\n  - name: x-participant-id\n    type: apiKey\n    in: header\n    parameter_name: x-participant-id\n    required: true\n    applies_to: Formulary Download API\n    description: >-\n      Participant ID of the requesting organization. Used\
  \ together with the mTLS client\n      certificate to determine the NCPDP Formulary & Benefit version(s) available, the\n      preferred drug database, and per-file permission restrictions.\n    sources:\n      - https://docs.surescripts.com/formulary-download/guide/api-details\n      - https://docs.surescripts.com/formulary-download/guide/security-and-data-access\n  - name: X-SENDER-UID\n    type: apiKey\n    in: header\n    parameter_name: X-SENDER-UID\n    required: true\n    applies_to: Medication History for Populations FHIR API\n    description: >-\n      Participant ID of the sender, e.g. T00000000012345 (the leading T denotes a staging /\n      test participant). Accompanied by the mandatory X-SENDER-UID-QUALIFIER header, fixed\n      value 10.\n    sources:\n      - https://docs.surescripts.com/medhistory-populations/guide/http-request-headers\n  - name: X-SENDER-UID-QUALIFIER\n    type: apiKey\n    in: header\n    parameter_name: X-SENDER-UID-QUALIFIER\n    required: true\n \
  \   fixed_value: '10'\n    applies_to: Medication History for Populations FHIR API\n    sources:\n      - https://docs.surescripts.com/medhistory-populations/guide/http-request-headers\nauthorization:\n  model: participant-entitlement\n  description: >-\n    Authorization is not scope-based. Entitlement is configured by Surescripts per Participant\n    ID during onboarding: which products the participant may call, which NCPDP F&B versions it\n    may read, and which files/resource IDs it may retrieve. A request that is authenticated but\n    not entitled returns 403 (Formulary Download 403-01/403-02/403-03; FHIR \"Product is not set\n    up for this participant ID\").\nfailure_modes:\n  - condition: No client certificate presented\n    result: SSL Connect Error (connection reset; no HTTP status)\n    remediation: Include the Surescripts-issued client certificate\n  - condition: Certificate issuer or subject does not match the configured certificate\n    result: 401 Unauthorized\n  - condition:\
  \ Certificate valid but participant not entitled to the product or resource\n    result: 403 Forbidden\nidentity_proofing:\n  required: true\n  note: >-\n    Identity Proofing Requirements and (for EPCS) a DEA third-party audit are pre-production\n    network requirements documented in the Connectivity and Operations section of the portal.\n    Those specific guides sit behind the portal's magic-link gate.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/surescripts/refs/heads/main/authentication/surescripts-authentication.yml
summary_line: mutualTLS/apiKey · 4 schemes
tags:
- Healthcare
- e-Prescribing
- Health Information Network
- NCPDP SCRIPT
- Medication History
- Prior Authorization
- Interoperability
- FHIR
- Formulary
- Eligibility
- Real-Time Prescription Benefit
- Mutual TLS
- Gated
---
