---
api_key_in: []
api_specs:
- filename: dcc-boxed-duis-signing-tool-openapi.yml
  format: yaml
  label: DCC Boxed DUIS Signing Tool API
  slug: dcc-boxed-duis-signing-tool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dcc-smart/refs/heads/main/openapi/dcc-boxed-duis-signing-tool-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Dcc Smart Authentication
name_suffix: Authentication
oauth_flows: []
overview: Smart DCC declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Smart DCC
provider_slug: dcc-smart
scheme_count: 0
schemes: []
slug: dcc-smart-authentication
source_filename: dcc-smart-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: https://github.com/SmartDCCInnovation/dccboxed-signing-tool\ndocs: https://smartenergycodecompany.co.uk/documents/sec-subsidiary-documents/sec-appendix-ae-dcc-user-interface-code-of-connection/\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    The one OpenAPI Smart DCC publishes declares NO securitySchemes. That is accurate,\n    not a gap in the spec: the DCC Boxed DUIS signing tool is a locally self-hosted\n    process bound to localhost:8080 with no authentication layer of its own. The real\n    Smart DCC production interface (DUIS) is not an API-key or OAuth surface at all — it\n    is a mutually-authenticated private network connection plus message-level PKI, and it\n    cannot be obtained self-serve.\nschemes: []\nsurfaces:\n- surface: DCC Boxed DUIS signing tool HTTP API\n  spec: openapi/dcc-boxed-duis-signing-tool-openapi.yml\n  auth: none\n  transport: plain HTTP on localhost (default port\
  \ 8080, configurable with -p)\n  note: >-\n    No authentication, no TLS by default. The tool is intended to run on the developer's\n    own machine or beside a DCC Boxed instance. The Node-RED nodes documentation notes\n    that DCC Boxed itself may be placed behind a reverse proxy performing authentication,\n    with extra headers and TLS configured on the client side — authentication is therefore\n    an operator concern, not a property of the published contract.\n- surface: DCC User Interface (DUIS) — the production Smart DCC interface\n  spec: null\n  auth: message-level XML digital signature with SMKI organisation certificates, over a\n    dedicated DCC User Gateway Connection\n  key_material: EC prime256v1 private keys in PKCS#8 PEM format, with the matching X.509\n    certificate in PEM, issued under SMKI (Smart Metering Key Infrastructure)\n  identity: the Originator and Target EUIs in the DUIS header identify the sending Remote\n    Party and the target device or ACB\n  replay_protection:\
  \ a strictly incrementing originator counter is carried in the DUIS\n    request id; the signing tool overwrites it with System.currentTimeMillis() unless\n    --preserveCounter is given\n  onboarding: >-\n    Not self-serve. Access requires acceding to the Smart Energy Code, ordering a DCC User\n    Gateway Connection, obtaining SMKI certificates, and passing SMKI Registration\n    Authority and User Entry Process Testing. Governed by SEC Appendix AE, the DCC User\n    Interface Code of Connection.\n  docs: https://smartenergycodecompany.co.uk/documents/sec-subsidiary-documents/sec-appendix-ae-dcc-user-interface-code-of-connection/\n- surface: DCC Boxed test PKI (ZAZ1)\n  auth: same SMKI XML digital signature model, using the ZAZ1 self-contained test PKI\n  note: >-\n    ZAZ1 organisation certificates and their private keys ship with DCC Boxed, with the\n    signing tool, and with GFI, and are published in the @smartdcc/dccboxed-keystore JSON\n    database. They are test credentials for\
  \ a test PKI — see sandbox/dcc-smart-sandbox.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dcc-smart/refs/heads/main/authentication/dcc-smart-authentication.yml
summary_line: 0 schemes
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Gas
- Smart Metering
- Grid
- Metering Infrastructure
- Energy Data
---
