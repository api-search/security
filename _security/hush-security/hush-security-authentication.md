---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Hush Security Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Hush Security secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Hush Security
provider_slug: hush-security
scheme_count: 1
schemes:
- client_authentication: http_basic
  credential_fields:
    api_key_id: HTTP Basic username
    api_key_secret: HTTP Basic password
  flow: clientCredentials
  grant_type: client_credentials
  name: OAuth2ClientCredentials
  optional_parameters:
  - description: Acts on behalf of an effective organization (the HTTPie plugin surfaces this as the EORG environment variable).
    location: token request body
    name: effective_org
  sources:
  - https://github.com/hushsecurity/httpie-hush
  - https://api.us.hush-security.com/v1/users
  token_response:
    access_token: 'bearer token used as Authorization: Bearer <access_token>'
    expires_in: token lifetime in seconds (short-lived, re-fetched on expiry)
  token_url: https://api.us.hush-security.com/v1/oauth/token
  type: oauth2
slug: hush-security-authentication
source_filename: hush-security-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.hush.security/knowledgebase/api\nnotes: >-\n  Auth model confirmed from the first-party HTTPie OAuth plugin\n  (github.com/hushsecurity/httpie-hush) and a live 401 challenge from\n  https://api.us.hush-security.com/v1/users. No public OpenAPI document was found\n  to derive securitySchemes mechanically, so this profile is hand-captured\n  (method: searched).\ndocs: https://docs.hush.security/knowledgebase/api\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  token_delivery: bearer\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://api.us.hush-security.com/v1/oauth/token\n  grant_type: client_credentials\n  client_authentication: http_basic\n  credential_fields:\n    api_key_id: HTTP Basic username\n    api_key_secret: HTTP Basic password\n  token_response:\n    access_token: 'bearer token used as Authorization: Bearer <access_token>'\n\
  \    expires_in: token lifetime in seconds (short-lived, re-fetched on expiry)\n  optional_parameters:\n  - name: effective_org\n    location: token request body\n    description: >-\n      Acts on behalf of an effective organization (the HTTPie plugin surfaces\n      this as the EORG environment variable).\n  sources:\n  - https://github.com/hushsecurity/httpie-hush\n  - https://api.us.hush-security.com/v1/users\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hush-security/refs/heads/main/authentication/hush-security-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Security
- Non-Human Identity
- Identity and Access Management
- Secrets Management
- AI Agents
- Agentic AI
- Kubernetes
- Cloud Security
- Workload Identity
---
