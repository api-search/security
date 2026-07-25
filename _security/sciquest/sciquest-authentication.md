---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Sciquest Authentication
name_suffix: Authentication
oauth_flows: []
overview: SciQuest declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: SciQuest
provider_slug: sciquest
scheme_count: 0
schemes: []
slug: sciquest-authentication
source_filename: sciquest-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  https://asodocs.jaggaer.com/ ;\n  https://www.jaggaer.com/wp-content/uploads/2024/06/JAGGAER-Integration-via-JAGGAER-Public-APIs.pdf\ntype: Authentication\nprovider: SciQuest / JAGGAER\napi: JAGGAER Advanced Sourcing Optimizer (ASO) API\ndocs: https://asodocs.jaggaer.com/\nsummary: >-\n  The JAGGAER (formerly SciQuest) ASO REST APIs are secured with OAuth 2.0 using\n  the client-credentials grant, letting a trusted server-side component obtain a\n  long-lived system-to-system bearer access token. Broader JAGGAER Public API\n  integrations additionally support cXML transactional messaging for\n  document-level exchange.\nsecurity_schemes:\n- id: oauth2_client_credentials\n  type: oauth2\n  flow: clientCredentials\n  description: >-\n    OAuth 2.0 Authorization using the Client Credential grant type; issues a\n    long-term system-to-system bearer access token presented as\n    Authorization: Bearer <token>.\n  token_placement:\
  \ header\n  header: Authorization\n  scheme: Bearer\n- id: cxml\n  type: message-signature\n  description: >-\n    cXML transactional messaging (credential/sender/receiver blocks) used for\n    punchout and document exchange in JAGGAER Public API integrations.\n  applies_to: JAGGAER Public API document exchange (not the ASO REST API)\nnotes: >-\n  Auth profile compiled from the ASO API documentation portal and JAGGAER's\n  public API integration guide. No OpenAPI securitySchemes block is published,\n  so this is a documentation-sourced profile rather than a spec derivation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sciquest/refs/heads/main/authentication/sciquest-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Enterprise Software
- Procurement
- E-Procurement
- Spend Management
- Source-to-Pay
- Supplier Management
- Sourcing
---
