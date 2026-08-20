---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Enboarder Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Enboarder secures its APIs with apiKey, oauth2, and http across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Enboarder
provider_slug: enboarder
scheme_count: 4
schemes:
- applies_to:
  - /restapi/v1/*
  - /reports/*
  description: 'Account-level API key sent in the `apikey` request header alongside `Content-Type: application/json`. Authenticates the v1 URI family (/restapi/v1/*, /reports/*). REST API access can be toggled on or off per account under Settings / Integration.'
  in: header
  name: apikey
  parameter_name: apikey
  sources:
  - https://help.enboarder.com/en/articles/4151199-enboarder-api-docs-authentication-overview
  type: apiKey
- applies_to:
  - /restapi/v2/*
  - /reports/v2/*
  description: OAuth 2.0 client credentials grant. Authenticates the v2 URI family (/restapi/v2/*, /reports/v2/*). The access token is sent in the `Authorization` header. The documentation states the token is valid for 1 hour.
  flow: clientCredentials
  name: oauth2-client-credentials
  scopes_documented:
  - api/workflow.basic
  - api/workflow.advance
  - api/settings.all
  sources:
  - https://help.enboarder.com/en/articles/4151199-enboarder-api-docs-authentication-overview
  token_urls:
  - region: AU
    url: https://auth.syd.e1.enboarder.com/oauth2/token
  - region: EU
    url: https://auth.fra.e1.enboarder.com/oauth2/token
  - region: US
    url: https://auth.ore.e1.enboarder.com/oauth2/token
  token_validity_seconds: 3600
  type: oauth2
- applies_to:
  - /scim/v2/*
  description: OAuth bearer token accepted on the SCIM 2.0 endpoints.
  name: scim-bearer
  scheme: bearer
  sources:
  - https://help.enboarder.com/en/articles/5890669-scim-api-user-provisioning-and-management
  type: http
- applies_to:
  - /scim/v2/*
  description: HTTP Basic authentication accepted on the SCIM 2.0 endpoints.
  name: scim-basic
  scheme: basic
  sources:
  - https://help.enboarder.com/en/articles/5890669-scim-api-user-provisioning-and-management
  type: http
slug: enboarder-authentication
source_filename: enboarder-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://help.enboarder.com/en/articles/4151199-enboarder-api-docs-authentication-overview\ndocs: https://help.enboarder.com/en/articles/4151199-enboarder-api-docs-authentication-overview\nnote: >-\n  Derived from the provider's published Authentication & Overview article and the SCIM\n  API article. Enboarder publishes no OpenAPI, so no securitySchemes could be read from\n  a machine-readable contract; every scheme below is transcribed from the documentation.\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  - http\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\n  transport: HTTPS only\nschemes:\n- name: apikey\n  type: apiKey\n  in: header\n  parameter_name: apikey\n  description: >-\n    Account-level API key sent in the `apikey` request header alongside\n    `Content-Type: application/json`. Authenticates the v1 URI family\n    (/restapi/v1/*, /reports/*). REST API access can be toggled on or off per account\n\
  \    under Settings / Integration.\n  applies_to:\n  - /restapi/v1/*\n  - /reports/*\n  sources:\n  - https://help.enboarder.com/en/articles/4151199-enboarder-api-docs-authentication-overview\n- name: oauth2-client-credentials\n  type: oauth2\n  flow: clientCredentials\n  description: >-\n    OAuth 2.0 client credentials grant. Authenticates the v2 URI family\n    (/restapi/v2/*, /reports/v2/*). The access token is sent in the `Authorization`\n    header. The documentation states the token is valid for 1 hour.\n  token_validity_seconds: 3600\n  token_urls:\n  - region: AU\n    url: https://auth.syd.e1.enboarder.com/oauth2/token\n  - region: EU\n    url: https://auth.fra.e1.enboarder.com/oauth2/token\n  - region: US\n    url: https://auth.ore.e1.enboarder.com/oauth2/token\n  scopes_documented:\n  - api/workflow.basic\n  - api/workflow.advance\n  - api/settings.all\n  applies_to:\n  - /restapi/v2/*\n  - /reports/v2/*\n  sources:\n  - https://help.enboarder.com/en/articles/4151199-enboarder-api-docs-authentication-overview\n\
  - name: scim-bearer\n  type: http\n  scheme: bearer\n  description: OAuth bearer token accepted on the SCIM 2.0 endpoints.\n  applies_to:\n  - /scim/v2/*\n  sources:\n  - https://help.enboarder.com/en/articles/5890669-scim-api-user-provisioning-and-management\n- name: scim-basic\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication accepted on the SCIM 2.0 endpoints.\n  applies_to:\n  - /scim/v2/*\n  sources:\n  - https://help.enboarder.com/en/articles/5890669-scim-api-user-provisioning-and-management\nregions:\n- region: AU\n  api_host: https://api.syd.e1.enboarder.com\n- region: EU\n  api_host: https://api.fra.e1.enboarder.com\n- region: US\n  api_host: https://api.ore.e1.enboarder.com\n- region: CA\n  api_host: https://api.can.e1.enboarder.com\ngaps:\n- No OIDC discovery document is served on the auth hosts (/.well-known/openid-configuration returns 404).\n- No RFC 8414 authorization-server metadata is served (/.well-known/oauth-authorization-server returns 404).\n\
  - No CA OAuth token host is published in the documentation; only AU, EU and US token URLs are listed.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enboarder/refs/heads/main/authentication/enboarder-authentication.yml
summary_line: apiKey/oauth2/http · 4 schemes
tags:
- Company
- Human Resources
- Employee Onboarding
- Employee Experience
- HR Technology
- Workflow-Automation
- SCIM
- Identity Provisioning
- Webhook
- Offboarding
---
