---
api_key_in: []
api_specs:
- filename: sedna-openapi.json
  format: json
  label: Sedna API
  slug: sedna-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-openapi.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Sedna Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: SEDNA secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: SEDNA
provider_slug: sedna
scheme_count: 2
schemes:
- description: The basic auth scheme only requires the API-Specific username/password to be set.
  name: Basic
  scheme: basic
  sources:
  - openapi/sedna-openapi.json
  type: http
- description: This API prefers OAuth 2 with client credentials flow. You can create your credentials in the <a href='https://{tenant}.sednanetwork.com/platform/settings/api-credential-management'>Api Credential Management page</a>.
  flows:
  - flow: clientCredentials
    scopes: 53
    tokenUrl: https://{tenant}.sednanetwork.com/platform/oauth/token
  name: OAuth
  sources:
  - openapi/sedna-openapi.json
  type: oauth2
slug: sedna-authentication
source_filename: sedna-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/sedna-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: Basic\n  type: http\n  scheme: basic\n  description: The basic auth scheme only requires the API-Specific username/password to be\n    set.\n  sources:\n  - openapi/sedna-openapi.json\n- name: OAuth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.sednanetwork.com/platform/oauth/token\n    scopes: 53\n  description: This API prefers OAuth 2 with client credentials flow. You can create your credentials\n    in the <a href='https://{tenant}.sednanetwork.com/platform/settings/api-credential-management'>Api\n    Credential Management page</a>.\n  sources:\n  - openapi/sedna-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/authentication/sedna-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Shipping
- Maritime
- Email
- Communications
- Workflow
- Commodity Trading
- Logistics
- Messaging
---
