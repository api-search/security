---
api_key_in: []
auth_types:
- scram
- http
description: ''
kind: authentication
layout: security
method: searched
name: Skyfoundry Authentication
name_suffix: Authentication
oauth_flows: []
overview: SkyFoundry secures its APIs with scram and http across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SkyFoundry
provider_slug: skyfoundry
scheme_count: 5
schemes:
- description: Salted Challenge Response Authentication Mechanism (RFC 5802) with SHA-256 (SHA-512 negotiable). All compliant Haystack HTTP API implementations, including SkySpark v3+, must support SCRAM. Client and server exchange base64url-encoded messages; the client proves password possession via PBKDF2 without transmitting the password.
  mechanism: SCRAM-SHA-256
  name: SCRAM
  required: true
  type: scram
- description: Transmits base64url-encoded credentials directly. MUST only be permitted over a secure TLS connection.
  name: PLAINTEXT
  required: false
  type: plaintext
- description: 'After a successful handshake the authToken issued in the Authentication-Info header is presented as "Authorization: BEARER authToken=...". SkySpark also accepts BASIC and DIGEST schemes for legacy clients where enabled.'
  name: BEARER
  scheme: bearer
  type: http
- description: HTTP Basic authentication, supported by SkySpark for legacy/simple clients over TLS where the server permits it.
  name: BASIC
  scheme: basic
  type: http
- description: HTTP Digest authentication, supported by SkySpark as a legacy mechanism.
  name: DIGEST
  scheme: digest
  type: http
slug: skyfoundry-authentication
source_filename: skyfoundry-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://project-haystack.org/doc/docHaystack/Auth\ndocs: https://project-haystack.org/doc/docHaystack/Auth\nnotes: >-\n  SkySpark is a native Project Haystack server and implements the Haystack HTTP\n  API authentication protocol. Authentication is a three-step exchange: a HELLO\n  handshake (client sends an Authorization header with the HELLO scheme and a\n  base64url-encoded username), a mechanism exchange (the server advertises\n  supported mechanisms via WWW-Authenticate), and token-based access. On success\n  the server returns 200 with an Authentication-Info header carrying an authToken;\n  clients then present \"Authorization: BEARER authToken=xxyyzz\" on subsequent\n  requests. Each SkySpark deployment is self-hosted, so there is no central\n  authorization server or public token endpoint — auth happens against the\n  customer's own SkySpark host at /ui or the /api/{proj} base.\nsummary:\n  types: [scram, http]\n  primary:\
  \ SCRAM-SHA-256\n  token: bearer-authtoken\nschemes:\n- name: SCRAM\n  type: scram\n  mechanism: SCRAM-SHA-256\n  required: true\n  description: >-\n    Salted Challenge Response Authentication Mechanism (RFC 5802) with SHA-256\n    (SHA-512 negotiable). All compliant Haystack HTTP API implementations, including\n    SkySpark v3+, must support SCRAM. Client and server exchange base64url-encoded\n    messages; the client proves password possession via PBKDF2 without transmitting\n    the password.\n- name: PLAINTEXT\n  type: plaintext\n  required: false\n  description: >-\n    Transmits base64url-encoded credentials directly. MUST only be permitted over a\n    secure TLS connection.\n- name: BEARER\n  type: http\n  scheme: bearer\n  description: >-\n    After a successful handshake the authToken issued in the Authentication-Info\n    header is presented as \"Authorization: BEARER authToken=...\". SkySpark also\n    accepts BASIC and DIGEST schemes for legacy clients where enabled.\n- name:\
  \ BASIC\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic authentication, supported by SkySpark for legacy/simple clients over\n    TLS where the server permits it.\n- name: DIGEST\n  type: http\n  scheme: digest\n  description: >-\n    HTTP Digest authentication, supported by SkySpark as a legacy mechanism.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skyfoundry/refs/heads/main/authentication/skyfoundry-authentication.yml
summary_line: scram/http · 5 schemes
tags:
- Company
- Building Analytics
- IoT
- Energy Management
- Fault Detection
- Smart Buildings
- Project Haystack
- Time Series
- Analytics
---
