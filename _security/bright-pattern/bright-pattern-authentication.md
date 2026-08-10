---
api_key_in: []
api_specs:
- filename: bright-pattern-authentication-api-openapi.yml
  format: yaml
  label: Bright Pattern Authentication API
  slug: bright-pattern-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-pattern/refs/heads/main/openapi/bright-pattern-authentication-api-openapi.yml
- filename: bright-pattern-calling-list-api-openapi.yml
  format: yaml
  label: Bright Pattern Calling List API
  slug: bright-pattern-calling-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-pattern/refs/heads/main/openapi/bright-pattern-calling-list-api-openapi.yml
- filename: bright-pattern-campaigns-api-openapi.yml
  format: yaml
  label: Bright Pattern Campaigns API
  slug: bright-pattern-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-pattern/refs/heads/main/openapi/bright-pattern-campaigns-api-openapi.yml
- filename: bright-pattern-dnc-lists-api-openapi.yml
  format: yaml
  label: Bright Pattern DNC Lists API
  slug: bright-pattern-dnc-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-pattern/refs/heads/main/openapi/bright-pattern-dnc-lists-api-openapi.yml
- filename: bright-pattern-do-not-call-list-api-openapi.yml
  format: yaml
  label: Bright Pattern Do Not Call List API
  slug: bright-pattern-do-not-call-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-pattern/refs/heads/main/openapi/bright-pattern-do-not-call-list-api-openapi.yml
- filename: bright-pattern-link-groups-api-openapi.yml
  format: yaml
  label: Bright Pattern Link Groups API
  slug: bright-pattern-link-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-pattern/refs/heads/main/openapi/bright-pattern-link-groups-api-openapi.yml
- filename: bright-pattern-lists-api-openapi.yml
  format: yaml
  label: Bright Pattern Lists API
  slug: bright-pattern-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-pattern/refs/heads/main/openapi/bright-pattern-lists-api-openapi.yml
- filename: bright-pattern-methods-api-openapi.yml
  format: yaml
  label: Bright Pattern Methods API
  slug: bright-pattern-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-pattern/refs/heads/main/openapi/bright-pattern-methods-api-openapi.yml
- filename: bright-pattern-multichannel-call-recordings-api-openapi.yml
  format: yaml
  label: Bright Pattern Multichannel Call Recordings API
  slug: bright-pattern-multichannel-call-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-pattern/refs/heads/main/openapi/bright-pattern-multichannel-call-recordings-api-openapi.yml
- filename: bright-pattern-phones-api-openapi.yml
  format: yaml
  label: Bright Pattern Phones API
  slug: bright-pattern-phones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-pattern/refs/heads/main/openapi/bright-pattern-phones-api-openapi.yml
- filename: bright-pattern-regular-call-recordings-api-openapi.yml
  format: yaml
  label: Bright Pattern Regular Call Recordings API
  slug: bright-pattern-regular-call-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-pattern/refs/heads/main/openapi/bright-pattern-regular-call-recordings-api-openapi.yml
- filename: bright-pattern-sms-mms-messaging-api-openapi.yml
  format: yaml
  label: Bright Pattern SMS/MMS Messaging API
  slug: bright-pattern-sms-mms-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-pattern/refs/heads/main/openapi/bright-pattern-sms-mms-messaging-api-openapi.yml
- filename: bright-pattern-task-routing-api-openapi.yml
  format: yaml
  label: Bright Pattern Task Routing API
  slug: bright-pattern-task-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-pattern/refs/heads/main/openapi/bright-pattern-task-routing-api-openapi.yml
- filename: bright-pattern-users-api-openapi.yml
  format: yaml
  label: Bright Pattern Users API
  slug: bright-pattern-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-pattern/refs/heads/main/openapi/bright-pattern-users-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Bright Pattern Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Bright Pattern secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Bright Pattern
provider_slug: bright-pattern
scheme_count: 2
schemes:
- description: 'OAuth 2.0 access token issued by the Bright Pattern token endpoint, sent as `Authorization: Bearer <token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/bright-pattern-configuration-openapi.yml
  - openapi/bright-pattern-interaction-content-openapi.yml
  - openapi/bright-pattern-list-management-v2-openapi.yml
  - openapi/bright-pattern-list-management-v3-2-openapi.yml
  - openapi/bright-pattern-list-management-v3-openapi.yml
  - openapi/bright-pattern-mobile-web-messaging-v1-openapi.yml
  - openapi/bright-pattern-mobile-web-messaging-v2-openapi.yml
  - openapi/bright-pattern-real-time-statistics-openapi.yml
  - openapi/bright-pattern-scim-user-provisioning-openapi.yml
  - openapi/bright-pattern-sms-mms-openapi.yml
  - openapi/bright-pattern-task-routing-openapi.yml
  type: http
- description: OAuth 2.0 client-credentials grant against the Bright Pattern tenant token endpoint.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://{tenant_url}/configapi/v2/oauth/token
  name: oauth2ClientCredentials
  sources:
  - openapi/bright-pattern-configuration-openapi.yml
  - openapi/bright-pattern-interaction-content-openapi.yml
  - openapi/bright-pattern-list-management-v2-openapi.yml
  - openapi/bright-pattern-list-management-v3-2-openapi.yml
  - openapi/bright-pattern-list-management-v3-openapi.yml
  - openapi/bright-pattern-real-time-statistics-openapi.yml
  - openapi/bright-pattern-scim-user-provisioning-openapi.yml
  - openapi/bright-pattern-sms-mms-openapi.yml
  - openapi/bright-pattern-task-routing-openapi.yml
  type: oauth2
slug: bright-pattern-authentication
source_filename: bright-pattern-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: derived\nsource: openapi/bright-pattern-configuration-openapi.yml, openapi/bright-pattern-interaction-content-openapi.yml,\n  openapi/bright-pattern-list-management-v2-openapi.yml, openapi/bright-pattern-list-management-v3-2-openapi.yml,\n  openapi/bright-pattern-list-management-v3-openapi.yml, openapi/bright-pattern-mobile-web-messaging-v1-openapi.yml,\n  openapi/bright-pattern-mobile-web-messaging-v2-openapi.yml, openapi/bright-pattern-real-time-statistics-openapi.yml,\n  openapi/bright-pattern-scim-user-provisioning-openapi.yml, openapi/bright-pattern-sms-mms-openapi.yml,\n  openapi/bright-pattern-task-routing-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'OAuth 2.0 access token issued by the Bright Pattern token endpoint, sent as\n    `Authorization: Bearer <token>`.'\n  sources:\n  - openapi/bright-pattern-configuration-openapi.yml\n\
  \  - openapi/bright-pattern-interaction-content-openapi.yml\n  - openapi/bright-pattern-list-management-v2-openapi.yml\n  - openapi/bright-pattern-list-management-v3-2-openapi.yml\n  - openapi/bright-pattern-list-management-v3-openapi.yml\n  - openapi/bright-pattern-mobile-web-messaging-v1-openapi.yml\n  - openapi/bright-pattern-mobile-web-messaging-v2-openapi.yml\n  - openapi/bright-pattern-real-time-statistics-openapi.yml\n  - openapi/bright-pattern-scim-user-provisioning-openapi.yml\n  - openapi/bright-pattern-sms-mms-openapi.yml\n  - openapi/bright-pattern-task-routing-openapi.yml\n- name: oauth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant_url}/configapi/v2/oauth/token\n    scopes: 0\n  description: OAuth 2.0 client-credentials grant against the Bright Pattern tenant token endpoint.\n  sources:\n  - openapi/bright-pattern-configuration-openapi.yml\n  - openapi/bright-pattern-interaction-content-openapi.yml\n  - openapi/bright-pattern-list-management-v2-openapi.yml\n\
  \  - openapi/bright-pattern-list-management-v3-2-openapi.yml\n  - openapi/bright-pattern-list-management-v3-openapi.yml\n  - openapi/bright-pattern-real-time-statistics-openapi.yml\n  - openapi/bright-pattern-scim-user-provisioning-openapi.yml\n  - openapi/bright-pattern-sms-mms-openapi.yml\n  - openapi/bright-pattern-task-routing-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bright-pattern/refs/heads/main/authentication/bright-pattern-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Contact Center
- CCaaS
- Customer Experience
- Omnichannel
- Call Center
- Telephony
- Messaging
- SMS
- Voice
- Customer Service
- Workforce Management
---
