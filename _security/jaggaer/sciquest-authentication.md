---
anonymous_access: false
api_key_in: []
api_specs:
- filename: jaggaer-async-api-openapi.yml
  format: yaml
  label: JAGGAER Async API
  slug: jaggaer-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-async-api-openapi.yml
- filename: jaggaer-attributes-api-openapi.yml
  format: yaml
  label: JAGGAER Attributes API
  slug: jaggaer-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-attributes-api-openapi.yml
- filename: jaggaer-awards-api-openapi.yml
  format: yaml
  label: JAGGAER Awards API
  slug: jaggaer-awards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-awards-api-openapi.yml
- filename: jaggaer-bids-api-openapi.yml
  format: yaml
  label: JAGGAER Bids API
  slug: jaggaer-bids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-bids-api-openapi.yml
- filename: jaggaer-contacts-api-openapi.yml
  format: yaml
  label: JAGGAER Contacts API
  slug: jaggaer-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-contacts-api-openapi.yml
- filename: jaggaer-customer-hosts-api-openapi.yml
  format: yaml
  label: JAGGAER Customer Hosts API
  slug: jaggaer-customer-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-customer-hosts-api-openapi.yml
- filename: jaggaer-events-api-openapi.yml
  format: yaml
  label: JAGGAER Events API
  slug: jaggaer-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-events-api-openapi.yml
- filename: jaggaer-items-api-openapi.yml
  format: yaml
  label: JAGGAER Items API
  slug: jaggaer-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-items-api-openapi.yml
- filename: jaggaer-jobs-api-openapi.yml
  format: yaml
  label: JAGGAER Jobs API
  slug: jaggaer-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-jobs-api-openapi.yml
- filename: jaggaer-locations-api-openapi.yml
  format: yaml
  label: JAGGAER Locations API
  slug: jaggaer-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-locations-api-openapi.yml
- filename: jaggaer-rates-api-openapi.yml
  format: yaml
  label: JAGGAER Rates API
  slug: jaggaer-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-rates-api-openapi.yml
- filename: jaggaer-scenarios-api-openapi.yml
  format: yaml
  label: JAGGAER Scenarios API
  slug: jaggaer-scenarios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-scenarios-api-openapi.yml
- filename: jaggaer-suppliers-api-openapi.yml
  format: yaml
  label: JAGGAER Suppliers API
  slug: jaggaer-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-suppliers-api-openapi.yml
- filename: jaggaer-templates-api-openapi.yml
  format: yaml
  label: JAGGAER Templates API
  slug: jaggaer-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-templates-api-openapi.yml
- filename: jaggaer-uploads-api-openapi.yml
  format: yaml
  label: JAGGAER Uploads API
  slug: jaggaer-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-uploads-api-openapi.yml
- filename: jaggaer-users-api-openapi.yml
  format: yaml
  label: JAGGAER Users API
  slug: jaggaer-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/openapi/jaggaer-users-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Sciquest Authentication
name_suffix: Authentication
oauth_flows: []
overview: JAGGAER declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: JAGGAER
provider_slug: jaggaer
scheme_count: 0
schemes: []
slug: sciquest-authentication
source_filename: sciquest-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  https://asodocs.jaggaer.com/ ;\n  https://www.jaggaer.com/wp-content/uploads/2024/06/JAGGAER-Integration-via-JAGGAER-Public-APIs.pdf\ntype: Authentication\nprovider: SciQuest / JAGGAER\napi: JAGGAER Advanced Sourcing Optimizer (ASO) API\ndocs: https://asodocs.jaggaer.com/\nsummary: >-\n  The JAGGAER (formerly SciQuest) ASO REST APIs are secured with OAuth 2.0 using\n  the client-credentials grant, letting a trusted server-side component obtain a\n  long-lived system-to-system bearer access token. Broader JAGGAER Public API\n  integrations additionally support cXML transactional messaging for\n  document-level exchange.\nsecurity_schemes:\n- id: oauth2_client_credentials\n  type: oauth2\n  flow: clientCredentials\n  description: >-\n    OAuth 2.0 Authorization using the Client Credential grant type; issues a\n    long-term system-to-system bearer access token presented as\n    Authorization: Bearer <token>.\n  token_placement:\
  \ header\n  header: Authorization\n  scheme: Bearer\n- id: cxml\n  type: message-signature\n  description: >-\n    cXML transactional messaging (credential/sender/receiver blocks) used for\n    punchout and document exchange in JAGGAER Public API integrations.\n  applies_to: JAGGAER Public API document exchange (not the ASO REST API)\nnotes: >-\n  Auth profile compiled from the ASO API documentation portal and JAGGAER's\n  public API integration guide. No OpenAPI securitySchemes block is published,\n  so this is a documentation-sourced profile rather than a spec derivation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jaggaer/refs/heads/main/authentication/sciquest-authentication.yml
summary_line: 0 schemes
tags:
- Procurement
- Sourcing
- Supplier Management
- Contracts
- Spend Analytics
- eProcurement
- Source-to-Pay
- Procure-to-Pay
---
