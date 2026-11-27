---
anonymous_access: false
api_key_in: []
auth_types: []
description: OAuth 2.0 Client Credentials flow
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Enhesa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Enhesa declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Enhesa
provider_slug: enhesa
scheme_count: 1
schemes:
- evidence: All requests use OAuth 2.0 ClientCredentials. Each token is issued for one Enhesa Client at a time, following the principle of least privilege.
  flows:
  - client_credentials
  how_to_obtain: Contact services@enhesa.com to receive your OAuth 2.0 credentials (client_id, client_secret, enhesaclientid). Then exchange them for a token via the token endpoint.
  name: OAuth 2.0 Client Credentials
  scopes:
  - compliance_intelligence_api:read
  token_url: https://identity.enhesa.com/connect/token
  type: oauth2
slug: enhesa-authentication
source_filename: enhesa-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.enhesa.com/compliance-intelligence#authentication
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.enhesa.com/compliance-intelligence#authentication\nsources:\n- https://docs.enhesa.com/compliance-intelligence#authentication\n- https://docs.enhesa.com/compliance-intelligence\n- https://docs.enhesa.com/compliance-intelligence#getting-started\ndescription: OAuth 2.0 Client Credentials flow\nschemes:\n- type: oauth2\n  name: OAuth 2.0 Client Credentials\n  evidence: All requests use OAuth 2.0 ClientCredentials. Each token is issued for one Enhesa Client at a time, following the principle of least\n    privilege.\n  flows:\n  - client_credentials\n  token_url: https://identity.enhesa.com/connect/token\n  scopes:\n  - compliance_intelligence_api:read\n  how_to_obtain: Contact services@enhesa.com to receive your OAuth 2.0 credentials (client_id, client_secret, enhesaclientid). Then exchange them\n    for a token via the token endpoint.\nnote: 'All API calls must include\
  \ an Authorization header: Authorization: Bearer <access_token>.'\ndocs: https://docs.enhesa.com/compliance-intelligence#authentication\n"
source_yaml_url: https://artifacts.apis.io/enhesa/authentication/enhesa-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Compliance
- Environmental
- Sustainability
---
