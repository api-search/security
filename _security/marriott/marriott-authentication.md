---
api_key_in: []
api_specs:
- filename: marriott-actuator-api-openapi.yml
  format: yaml
  label: Marriott International Actuator API
  slug: marriott-actuator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-actuator-api-openapi.yml
- filename: marriott-auth-api-openapi.yml
  format: yaml
  label: Marriott International Auth API
  slug: marriott-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-auth-api-openapi.yml
- filename: marriott-data-api-openapi.yml
  format: yaml
  label: Marriott International Data API
  slug: marriott-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-data-api-openapi.yml
- filename: marriott-data-collection-event-api-openapi.yml
  format: yaml
  label: Marriott International Data Collection Event API
  slug: marriott-data-collection-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-data-collection-event-api-openapi.yml
- filename: marriott-freedompay-freeway-service-api-openapi.yml
  format: yaml
  label: Marriott International FreedomPay Freeway Service API
  slug: marriott-freedompay-freeway-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-freedompay-freeway-service-api-openapi.yml
- filename: marriott-guest-validation-api-openapi.yml
  format: yaml
  label: Marriott International Guest Validation API
  slug: marriott-guest-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-guest-validation-api-openapi.yml
- filename: marriott-internet-purchase-update-api-openapi.yml
  format: yaml
  label: Marriott International Internet Purchase Update API
  slug: marriott-internet-purchase-update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-internet-purchase-update-api-openapi.yml
- filename: marriott-landing-page-api-openapi.yml
  format: yaml
  label: Marriott International Landing Page API
  slug: marriott-landing-page-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-landing-page-api-openapi.yml
- filename: marriott-loyalty-api-openapi.yml
  format: yaml
  label: Marriott International Loyalty API
  slug: marriott-loyalty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-loyalty-api-openapi.yml
- filename: marriott-postpreviewsubmit-api-openapi.yml
  format: yaml
  label: Marriott International Post Preview Submit API
  slug: marriott-postpreviewsubmit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-postpreviewsubmit-api-openapi.yml
- filename: marriott-retrieveconfigsmonitoredbyconfigwatcher-api-openapi.yml
  format: yaml
  label: Marriott International Retrieve Configs Monitored By Config Watcher API
  slug: marriott-retrieveconfigsmonitoredbyconfigwatcher-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-retrieveconfigsmonitoredbyconfigwatcher-api-openapi.yml
- filename: marriott-status-api-openapi.yml
  format: yaml
  label: Marriott International Status API
  slug: marriott-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/openapi/marriott-status-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Marriott Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Marriott International secures its APIs with http and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Marriott International
provider_slug: marriott
scheme_count: 4
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/marriott-commerce-payment-processor-api-openapi.json
  - openapi/marriott-tip-internet-portal-api-openapi.json
  type: http
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/marriott-commerce-payment-processor-api-openapi.json
  - openapi/marriott-tip-internet-portal-api-openapi.json
  type: http
- flows:
  - authorizationUrl: /v3/ent-auth/sso/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: /v3/ent-auth/sso/token
  name: OAuth2
  sources:
  - openapi/marriott-commerce-payment-processor-api-openapi.json
  type: oauth2
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: http://example.com/oauth/token
  name: application
  sources:
  - openapi/marriott-finance-status-notifier-api-openapi.json
  type: oauth2
slug: marriott-authentication
source_filename: marriott-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: derived\nsource: openapi/marriott-commerce-payment-processor-api-openapi.json, openapi/marriott-finance-status-notifier-api-openapi.json,\n  openapi/marriott-tip-internet-portal-api-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/marriott-commerce-payment-processor-api-openapi.json\n  - openapi/marriott-tip-internet-portal-api-openapi.json\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/marriott-commerce-payment-processor-api-openapi.json\n  - openapi/marriott-tip-internet-portal-api-openapi.json\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /v3/ent-auth/sso/authorize\n    tokenUrl: /v3/ent-auth/sso/token\n    scopes: 1\n  sources:\n  - openapi/marriott-commerce-payment-processor-api-openapi.json\n\
  - name: application\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: http://example.com/oauth/token\n    scopes: 1\n  sources:\n  - openapi/marriott-finance-status-notifier-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marriott/refs/heads/main/authentication/marriott-authentication.yml
summary_line: http/oauth2 · 4 schemes
tags:
- Travel
- United States
- Hospitality
- Hotels
- Booking
- Distribution
- Loyalty
- Short Term Rental
- Corporate Travel
---
