---
api_key_in: []
api_specs:
- filename: nedap-ons-openapi-original.json
  format: json
  label: Nedap Ons API
  slug: nedap-ons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nedap/refs/heads/main/openapi/nedap-ons-openapi-original.json
auth_types:
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Nedap Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nedap secures its APIs with mutualTLS across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nedap
provider_slug: nedap
scheme_count: 1
schemes:
- ca_chains:
    development: https://ons-api.nl/assets/development-chain.pem
    legacy_note: Separate legacy chains are published for certificates signed before 02-09-2025 (production), 28-08-2025 (staging) and 20-08-2025 (development); no new certificates are issued from them.
    production: https://ons-api.nl/assets/production-chain.pem
    staging: https://ons-api.nl/assets/staging-chain.pem
  documented_only: true
  issuance:
    authority: Nedap's own Certificate Authority (per environment)
    cn_example: hr_integration-TE1002-free_text
    csr_requirements:
    - Key length of at least 4096 bits
    - CN, OU, O, L, ST, C and email address all filled in
    - CN structured as {technical_name_connector}-{customer_code}-{identification}
    process: Generate a 4096-bit CSR, upload it to the Ons API Dashboard, receive a signed PEM back. The private key is never shared with Nedap; if it leaks, the certificate is disabled in the Dashboard.
  name: OnsApiClientCertificate
  sources:
  - https://ons-api.nl/english/technical/Certificate_requirements.html
  transport:
    ciphers:
    - ECDHE-ECDSA-AES256-GCM-SHA384
    - ECDHE-ECDSA-AES128-GCM-SHA256
    - ECDHE-ECDSA-CHACHA20-POLY1305
    - ECDHE-RSA-AES256-GCM-SHA384
    - ECDHE-RSA-AES128-GCM-SHA256
    - ECDHE-RSA-CHACHA20-POLY1305
    - DHE-RSA-AES256-GCM-SHA384
    - DHE-RSA-AES128-GCM-SHA256
    min_tls: TLSv1.2
    sni_required: true
  type: mutualTLS
  verification:
    endpoint: GET /ping
    expected: 200 = the certificate works; 403 = the certificate does not work with this URL
slug: nedap-authentication
source_filename: nedap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: openapi/nedap-ons-openapi-original.json\ndocs: https://ons-api.nl/english/technical/Certificate_requirements.html\napi: Nedap Ons API\nnote: >-\n  The harvested OpenAPI declares no components.securitySchemes at all — running\n  derive-authentication.py over it yields nothing — so this profile is read from the\n  docs instead. Ons API is mutual-TLS only. There is no bearer token, no API key and no\n  OAuth: every request must be made with an SSL client certificate signed by Nedap's\n  own Certificate Authority, and that certificate binds one connector to one customer\n  environment. That is the strongest auth posture in this pipeline and the least\n  agent-reachable one — an agent cannot self-serve a credential; a human completes an\n  intake, has a connector reviewed, submits a CSR and receives a PEM back.\nsummary:\n  types:\n  - mutualTLS\n  api_key_in: []\n  oauth2_flows: []\n  self_serve: false\n  spec_declares_security:\
  \ false\nschemes:\n- name: OnsApiClientCertificate\n  type: mutualTLS\n  documented_only: true\n  sources:\n  - https://ons-api.nl/english/technical/Certificate_requirements.html\n  issuance:\n    authority: Nedap's own Certificate Authority (per environment)\n    process: >-\n      Generate a 4096-bit CSR, upload it to the Ons API Dashboard, receive a signed PEM\n      back. The private key is never shared with Nedap; if it leaks, the certificate is\n      disabled in the Dashboard.\n    csr_requirements:\n    - Key length of at least 4096 bits\n    - CN, OU, O, L, ST, C and email address all filled in\n    - 'CN structured as {technical_name_connector}-{customer_code}-{identification}'\n    cn_example: hr_integration-TE1002-free_text\n  transport:\n    min_tls: TLSv1.2\n    sni_required: true\n    ciphers:\n    - ECDHE-ECDSA-AES256-GCM-SHA384\n    - ECDHE-ECDSA-AES128-GCM-SHA256\n    - ECDHE-ECDSA-CHACHA20-POLY1305\n    - ECDHE-RSA-AES256-GCM-SHA384\n    - ECDHE-RSA-AES128-GCM-SHA256\n\
  \    - ECDHE-RSA-CHACHA20-POLY1305\n    - DHE-RSA-AES256-GCM-SHA384\n    - DHE-RSA-AES128-GCM-SHA256\n  ca_chains:\n    production: https://ons-api.nl/assets/production-chain.pem\n    staging: https://ons-api.nl/assets/staging-chain.pem\n    development: https://ons-api.nl/assets/development-chain.pem\n    legacy_note: >-\n      Separate legacy chains are published for certificates signed before 02-09-2025\n      (production), 28-08-2025 (staging) and 20-08-2025 (development); no new\n      certificates are issued from them.\n  verification:\n    endpoint: GET /ping\n    expected: '200 = the certificate works; 403 = the certificate does not work with this URL'\nauthorization:\n  model: Ons Autorisatie rights, evaluated per user/employee per client\n  note: >-\n    Authorization is not OAuth scopes. It is Nedap's own rights model, and a connector\n    queries it rather than carrying it in a token. Four read operations expose it —\n    scopeForUser, scopeForEmployee, clearanceForUser, clearanceForEmployee\
  \ — returning\n    either the set of client ids a user may reach for a named right, or a boolean\n    clearance for one client. A right not linked to the connector's version yields 404.\n  spec: openapi/nedap-ons-authorization-openapi-original.json\n  docs: https://ons-api.nl/english/authorization/UsingAuthorizationAPIs.html\n  operations:\n  - scopeForUser\n  - scopeForEmployee\n  - clearanceForUser\n  - clearanceForEmployee\nidentity_headers:\n- name: X-Cupido-User-Name\n  used_by: 130 operations\n  note: Names the acting user behind the connector; feeds Ons' own audit trail.\n- name: X-Cupido-Active-Identity\n  used_by: 127 operations\nwebhooks:\n  method: HMAC\n  note: >-\n    Inbound webhook notifications are authenticated the other way round — the connector\n    generates a secret in the Ons API Dashboard and verifies a Hash-based Message\n    Authentication Code on each POST, answering 200 for a valid HMAC and 401 for an\n    invalid one. Nedap sends two NOP events at configuration\
  \ time, one with a correct\n    HMAC and one with a deliberately wrong one, to prove the receiver checks.\n  docs: https://ons-api.nl/english/technical/Webhooks.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nedap/refs/heads/main/authentication/nedap-authentication.yml
summary_line: mutualTLS · 1 scheme
tags:
- Company
- Healthcare
- Electronic Health Records
- Interoperability
- FHIR
- openEHR
- RFID
- Retail
- Physical Security
- Livestock
- Netherlands
- Webhooks
---
