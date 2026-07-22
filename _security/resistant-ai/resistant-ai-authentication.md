---
api_key_in: []
api_specs:
- filename: resistant-ai-documents-openapi.json
  format: json
  label: Resistant Documents API
  slug: resistant-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resistant-ai/refs/heads/main/openapi/resistant-ai-documents-openapi.json
- filename: resistant-ai-tenant-management-openapi.json
  format: json
  label: Resistant Documents Tenant Management API
  slug: resistant-documents-tenant-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resistant-ai/refs/heads/main/openapi/resistant-ai-tenant-management-openapi.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Resistant Ai Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Resistant AI secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Resistant AI
provider_slug: resistant-ai
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://eu.id.resistant.ai/oauth2/aus2un1hkrKhPjir4417/v1/token
  name: OAuth2
  sources:
  - openapi/resistant-ai-documents-openapi.json
  type: oauth2
slug: resistant-ai-authentication
source_filename: resistant-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/resistant-ai-documents-openapi.json\ndocs: https://developers.resistant.ai/getting-started/authentication\nnotes:\n- 'OAuth2 client-credentials. Token obtained by POSTing HTTP Basic (client_id:client_secret) to the\n  cell token URL with grant_type=client_credentials. Access token sent as the Authorization Bearer header.'\n- Identity issuer eu.id.resistant.ai (Okta-hosted) publishes /.well-known/openid-configuration.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://eu.id.resistant.ai/oauth2/aus2un1hkrKhPjir4417/v1/token\n    scopes: 2\n  sources:\n  - openapi/resistant-ai-documents-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/resistant-ai/refs/heads/main/authentication/resistant-ai-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Ai
- Fraud Detection
- Financial Crime
- Document Verification
- Document Forensics
- AML
- Identity Verification
- Fintech
- Machine Learning
---
