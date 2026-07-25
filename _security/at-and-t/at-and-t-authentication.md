---
api_key_in:
- header
api_specs:
- filename: at-and-t-authentication-api-openapi.yml
  format: yaml
  label: AT&T Authentication API
  slug: at-and-t-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/openapi/at-and-t-authentication-api-openapi.yml
- filename: at-and-t-balance-management-api-openapi.yml
  format: yaml
  label: AT&T Balance Management API
  slug: at-and-t-balance-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/openapi/at-and-t-balance-management-api-openapi.yml
- filename: at-and-t-device-management-api-openapi.yml
  format: yaml
  label: AT&T Device Management API
  slug: at-and-t-device-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/openapi/at-and-t-device-management-api-openapi.yml
- filename: at-and-t-geographic-sites-api-openapi.yml
  format: yaml
  label: AT&T Geographic Sites API
  slug: at-and-t-geographic-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/openapi/at-and-t-geographic-sites-api-openapi.yml
- filename: at-and-t-inbox-management-api-openapi.yml
  format: yaml
  label: AT&T Inbox Management API
  slug: at-and-t-inbox-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/openapi/at-and-t-inbox-management-api-openapi.yml
- filename: at-and-t-messages-api-openapi.yml
  format: yaml
  label: AT&T Messages API
  slug: at-and-t-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/openapi/at-and-t-messages-api-openapi.yml
- filename: at-and-t-number-management-api-openapi.yml
  format: yaml
  label: AT&T Number Management API
  slug: at-and-t-number-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/openapi/at-and-t-number-management-api-openapi.yml
- filename: at-and-t-porting-api-openapi.yml
  format: yaml
  label: AT&T Porting API
  slug: at-and-t-porting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/openapi/at-and-t-porting-api-openapi.yml
- filename: at-and-t-product-orders-api-openapi.yml
  format: yaml
  label: AT&T Product Orders API
  slug: at-and-t-product-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/openapi/at-and-t-product-orders-api-openapi.yml
- filename: at-and-t-service-management-api-openapi.yml
  format: yaml
  label: AT&T Service Management API
  slug: at-and-t-service-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/openapi/at-and-t-service-management-api-openapi.yml
- filename: at-and-t-sms-messaging-api-openapi.yml
  format: yaml
  label: AT&T SMS Messaging API
  slug: at-and-t-sms-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/openapi/at-and-t-sms-messaging-api-openapi.yml
- filename: at-and-t-subscriber-management-api-openapi.yml
  format: yaml
  label: AT&T Subscriber Management API
  slug: at-and-t-subscriber-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/openapi/at-and-t-subscriber-management-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: At And T Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: AT&T secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: AT&T
provider_slug: at-and-t
scheme_count: 3
schemes:
- description: AT&T OAuth 2.0 with user consent via authorization code flow
  flows:
  - authorizationUrl: https://api.att.com/oauth/v4/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://api.att.com/oauth/v4/token
  name: oauth2
  sources:
  - openapi/at-and-t-in-app-messaging-api.yaml
  type: oauth2
- description: Client ID enforcement policy for MVNX API authentication
  in: header
  name: clientId
  parameter: X-Client-Id
  sources:
  - openapi/at-and-t-mvnx-api.yaml
  type: apiKey
- description: AT&T OAuth 2.0 authentication using client credentials grant
  flows:
  - flow: clientCredentials
    scopes: 6
    tokenUrl: https://api.att.com/oauth/v4/token
  name: oauth2
  sources:
  - openapi/at-and-t-sms-api.yaml
  type: oauth2
slug: at-and-t-authentication
source_filename: at-and-t-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/at-and-t-in-app-messaging-api.yaml, openapi/at-and-t-mvnx-api.yaml, openapi/at-and-t-sms-api.yaml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.att.com/oauth/v4/authorize\n    tokenUrl: https://api.att.com/oauth/v4/token\n    scopes: 2\n  description: AT&T OAuth 2.0 with user consent via authorization code flow\n  sources:\n  - openapi/at-and-t-in-app-messaging-api.yaml\n- name: clientId\n  type: apiKey\n  in: header\n  parameter: X-Client-Id\n  description: Client ID enforcement policy for MVNX API authentication\n  sources:\n  - openapi/at-and-t-mvnx-api.yaml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.att.com/oauth/v4/token\n    scopes: 6\n  description: AT&T OAuth\
  \ 2.0 authentication using client credentials grant\n  sources:\n  - openapi/at-and-t-sms-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/authentication/at-and-t-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Fortune 100
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
---
