---
api_key_in:
- header
api_specs:
- filename: crossenagage-user-management-v2-openapi.yml
  format: yaml
  label: CrossEngage User Management API v2
  slug: user-management-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crossenagage/refs/heads/main/openapi/crossenagage-user-management-v2-openapi.yml
- filename: crossenagage-user-management-v1-openapi.yml
  format: yaml
  label: CrossEngage User Management API v1
  slug: user-management-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crossenagage/refs/heads/main/openapi/crossenagage-user-management-v1-openapi.yml
- filename: crossenagage-product-feed-openapi.yml
  format: yaml
  label: CrossEngage Product Feed API
  slug: product-feed
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crossenagage/refs/heads/main/openapi/crossenagage-product-feed-openapi.yml
- filename: crossenagage-raw-export-v1-openapi.yml
  format: yaml
  label: CrossEngage Raw Export API
  slug: raw-export
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crossenagage/refs/heads/main/openapi/crossenagage-raw-export-v1-openapi.yml
- filename: crossenagage-statistics-v1-openapi.yml
  format: yaml
  label: CrossEngage Statistics API
  slug: statistics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crossenagage/refs/heads/main/openapi/crossenagage-statistics-v1-openapi.yml
- filename: crossenagage-file-attachments-v1-openapi.yml
  format: yaml
  label: CrossEngage File Attachments API
  slug: file-attachments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crossenagage/refs/heads/main/openapi/crossenagage-file-attachments-v1-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Crossenagage Authentication
name_suffix: Authentication
oauth_flows: []
overview: CrossEngage secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CrossEngage
provider_slug: crossenagage
scheme_count: 1
schemes:
- description: CrossEngage header authentication. The API key is issued in the CrossEngage app under Settings -> System setup -> API keys (Master API key or Public API key depending on the API).
  in: header
  name: XngAuthToken
  parameter: X-XNG-AuthToken
  sources:
  - openapi/crossenagage-file-attachments-v1-openapi.yml
  - openapi/crossenagage-raw-export-v1-openapi.yml
  - openapi/crossenagage-statistics-v1-openapi.yml
  - openapi/crossenagage-user-management-v1-openapi.yml
  - openapi/crossenagage-user-management-v2-openapi.yml
  type: apiKey
slug: crossenagage-authentication
source_filename: crossenagage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: the \"Authentication\" and \"Headers\" sections of the six CrossEngage API contracts on Apiary, cross-checked\n  against openapi/ (6 specs)\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: XngAuthToken\n  type: apiKey\n  in: header\n  parameter: X-XNG-AuthToken\n  description: CrossEngage header authentication. The API key is issued in the CrossEngage app under Settings\n    -> System setup -> API keys (Master API key or Public API key depending on the API).\n  sources:\n  - openapi/crossenagage-file-attachments-v1-openapi.yml\n  - openapi/crossenagage-raw-export-v1-openapi.yml\n  - openapi/crossenagage-statistics-v1-openapi.yml\n  - openapi/crossenagage-user-management-v1-openapi.yml\n  - openapi/crossenagage-user-management-v2-openapi.yml\ndocs: https://usermanagementv2.docs.apiary.io/\nnote: 'CrossEngage uses static header authentication only — no OAuth, no OIDC, no mTLS. Two key TIERS\n  exist\
  \ and they are not interchangeable: the MASTER API key authorises User Management (v1 and v2), Product\n  Feed and Raw Export; the PUBLIC API key authorises Statistics and File Attachments. Both are issued\n  inside the authenticated app under Settings -> System setup -> API keys; there is no self-serve signup,\n  key rotation endpoint or programmatic key issuance. A second header, X-XNG-ApiVersion, is required on\n  every call and is a version selector rather than a credential — it is modelled as a parameter, not a\n  securityScheme.'\nkey_tiers:\n- tier: Master API key\n  header: X-XNG-AuthToken\n  apis:\n  - User Management v1\n  - User Management v2\n  - Product Feed v1\n  - Raw Export v1\n  source: https://usermanagementv2.docs.apiary.io/, https://productfeedapiv1.docs.apiary.io/, https://userseventsexportapiv1.docs.apiary.io/\n- tier: Public API key\n  header: X-XNG-AuthToken\n  apis:\n  - Statistics v1\n  - File Attachments v1\n  source: https://statisticsapi1.docs.apiary.io/, https://fileattachmentsv1.docs.apiary.io/\n\
  required_headers:\n- header: X-XNG-AuthToken\n  role: credential\n  required: true\n- header: X-XNG-ApiVersion\n  role: version selector\n  required: true\n  values:\n    User Management: 1 or 2\n    Product Feed: '1'\n    Raw Export: '2'\n    Statistics: '2'\n    File Attachments: '2'\ngaps:\n- no OAuth 2.0 or OIDC surface\n- no scopes or granular permissions on the API key\n- no programmatic key rotation or issuance\n- no /.well-known/oauth-authorization-server (404 on all four hosts)\n- no mTLS\n- no signed-request option\nobtaining_credentials:\n  self_serve: false\n  requires_account: true\n  path: CrossEngage app (https://app.crossengage.io) -> Settings -> System setup -> API keys\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crossenagage/refs/heads/main/authentication/crossenagage-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Customer Data Platform
- Marketing
- Customer Engagement
- Marketing Automation
- Cross-Channel
- Personalization
- Predictive Analytics
- Segmentation
- Campaign Management
- Product Feed
- Data Export
- Webhooks
- Web Tracking
- Germany
---
