---
api_key_in: []
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Web Methods Authentication
name_suffix: Authentication
oauth_flows: []
overview: Web Methods secures its APIs with http, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Web Methods
provider_slug: web-methods
scheme_count: 3
schemes:
- applies_to: Developer Portal REST APIs
  name: basicAuth
  scheme: basic
  source: https://docs.webmethods.io/api/10.11.0/webmethods_developer_portal/chapter10dpo/
  type: http
- applies_to: API Gateway / API Management managed APIs
  flows:
  - authorizationCode
  - clientCredentials
  name: oauth2
  source: https://www.linkedin.com/pulse/oauth2-webmethods-api-gateway-fabio-romana-pisciotta
  type: oauth2
- applies_to: API Gateway / API Management managed APIs
  name: openIdConnect
  source: https://docs.webmethods.io/
  type: openIdConnect
slug: web-methods-authentication
source_filename: web-methods-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.webmethods.io/\ndocs: https://docs.webmethods.io/api/10.11.0/webmethods_developer_portal/chapter10dpo/\nsummary:\n  types:\n  - http\n  - oauth2\n  - openIdConnect\n  notes: >-\n    webMethods exposes several REST surfaces with different auth models. The\n    Developer Portal REST APIs use HTTP Basic authentication. The webMethods /\n    IBM webMethods API Gateway and API Management support OAuth2 (client\n    credentials, authorization code) and OpenID Connect for securing managed\n    APIs, alongside API-key and mutual-TLS policies configurable per API.\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  applies_to: Developer Portal REST APIs\n  source: https://docs.webmethods.io/api/10.11.0/webmethods_developer_portal/chapter10dpo/\n- name: oauth2\n  type: oauth2\n  applies_to: API Gateway / API Management managed APIs\n  flows:\n  - authorizationCode\n  - clientCredentials\n  source: https://www.linkedin.com/pulse/oauth2-webmethods-api-gateway-fabio-romana-pisciotta\n\
  - name: openIdConnect\n  type: openIdConnect\n  applies_to: API Gateway / API Management managed APIs\n  source: https://docs.webmethods.io/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/web-methods/refs/heads/main/authentication/web-methods-authentication.yml
summary_line: http/oauth2/openIdConnect · 3 schemes
tags:
- Company
- Integration
- iPaaS
- API Management
- API Gateway
- Enterprise Integration
- B2B
- EDI
- Developer Portal
- Middleware
- ESB
- Event-Driven
---
