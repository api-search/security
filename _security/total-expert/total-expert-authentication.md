---
api_key_in: []
api_specs:
- filename: total-expert-account-endpoints-api-openapi.yml
  format: yaml
  label: Total Expert Account Endpoints API
  slug: total-expert-account-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-account-endpoints-api-openapi.yml
- filename: total-expert-activity-endpoints-api-openapi.yml
  format: yaml
  label: Total Expert Activity Endpoints API
  slug: total-expert-activity-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-activity-endpoints-api-openapi.yml
- filename: total-expert-alm-leads-formerly-lead-opportunities-api-openapi.yml
  format: yaml
  label: Total Expert ALM Leads (formerly Lead Opportunities) API
  slug: total-expert-alm-leads-formerly-lead-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-alm-leads-formerly-lead-opportunities-api-openapi.yml
- filename: total-expert-authentication-api-openapi.yml
  format: yaml
  label: Total Expert Authentication API
  slug: total-expert-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-authentication-api-openapi.yml
- filename: total-expert-contact-endpoints-api-openapi.yml
  format: yaml
  label: Total Expert Contact Endpoints API
  slug: total-expert-contact-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-contact-endpoints-api-openapi.yml
- filename: total-expert-email-apis-api-openapi.yml
  format: yaml
  label: Total Expert Email APIs API
  slug: total-expert-email-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-email-apis-api-openapi.yml
- filename: total-expert-email-unsubscribes-api-openapi.yml
  format: yaml
  label: Total Expert Email Unsubscribes API
  slug: total-expert-email-unsubscribes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-email-unsubscribes-api-openapi.yml
- filename: total-expert-entities-api-openapi.yml
  format: yaml
  label: Total Expert Entities API
  slug: total-expert-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-entities-api-openapi.yml
- filename: total-expert-heartbeat-api-openapi.yml
  format: yaml
  label: Total Expert Heartbeat API
  slug: total-expert-heartbeat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-heartbeat-api-openapi.yml
- filename: total-expert-insight-endpoints-api-openapi.yml
  format: yaml
  label: Total Expert Insight Endpoints API
  slug: total-expert-insight-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-insight-endpoints-api-openapi.yml
- filename: total-expert-lead-opportunities-new-api-openapi.yml
  format: yaml
  label: Total Expert Lead Opportunities (New) API
  slug: total-expert-lead-opportunities-new-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-lead-opportunities-new-api-openapi.yml
- filename: total-expert-loan-endpoints-api-openapi.yml
  format: yaml
  label: Total Expert Loan Endpoints API
  slug: total-expert-loan-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-loan-endpoints-api-openapi.yml
- filename: total-expert-scenarios-api-openapi.yml
  format: yaml
  label: Total Expert Scenarios API
  slug: total-expert-scenarios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-scenarios-api-openapi.yml
- filename: total-expert-schema-endpoints-api-openapi.yml
  format: yaml
  label: Total Expert Schema Endpoints API
  slug: total-expert-schema-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-schema-endpoints-api-openapi.yml
- filename: total-expert-sms-opting-api-openapi.yml
  format: yaml
  label: Total Expert SMS Opting API
  slug: total-expert-sms-opting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-sms-opting-api-openapi.yml
- filename: total-expert-user-endpoints-api-openapi.yml
  format: yaml
  label: Total Expert User Endpoints API
  slug: total-expert-user-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-user-endpoints-api-openapi.yml
- filename: total-expert-webhooks-api-openapi.yml
  format: yaml
  label: Total Expert Webhooks API
  slug: total-expert-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-webhooks-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Total Expert Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Total Expert secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Total Expert
provider_slug: total-expert
scheme_count: 1
schemes:
- description: OAuth 2.0. Obtain a token from POST /v1/token using HTTP Basic (client_id:client_secret base64-encoded) plus a grant_type body. Access tokens are bearer tokens, expires_in 3600.
  flows:
  - flow: clientCredentials
    scopes: 5
    tokenUrl: https://public.totalexpert.net/v1/token
  - authorizationUrl: https://public.totalexpert.net/v1/authorize
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://public.totalexpert.net/v1/token
  name: oauth2
  sources:
  - openapi/total-expert-openapi.yml
  type: oauth2
slug: total-expert-authentication
source_filename: total-expert-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/total-expert-openapi.yml\ndocs: https://public.totalexpert.net/v1/docs/OAuth+Authorization+Guide.pdf\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://public.totalexpert.net/v1/token\n    scopes: 5\n  - flow: authorizationCode\n    authorizationUrl: https://public.totalexpert.net/v1/authorize\n    tokenUrl: https://public.totalexpert.net/v1/token\n    scopes: 5\n  description: >-\n    OAuth 2.0. Obtain a token from POST /v1/token using HTTP Basic\n    (client_id:client_secret base64-encoded) plus a grant_type body. Access\n    tokens are bearer tokens, expires_in 3600.\n  sources:\n  - openapi/total-expert-openapi.yml\nnotes:\n  token_request_auth: >-\n    All /v1/token requests carry an Authorization header implementing HTTP Basic:\n    base64(\"clientId:clientSecret\"\
  ), per the Vendor OAuth Integration Guide.\n  grant_types: [client_credentials, authorization_code, refresh_token]\n  access_token_ttl: 3600 seconds (1 hour); best practice is to cache the token since the token endpoint is rate limited to 2 requests per hour.\n  refresh_token_ttl: up to 2 weeks (Getting Started guide)\n  admin_vs_user: >-\n    Client-credentials tokens make calls \"As Admin\"; authorization-code (user\n    login) tokens make calls \"As User\". Many endpoints document both request\n    shapes.\n  environments: >-\n    Production tokens come from public.totalexpert.net; the isolated\n    development/sandbox domain public.vt.totalexpert.net exposes the same\n    /v1/authorize and /v1/token endpoints with separate credentials.\n  redirect_uri: Must be preregistered with Total Expert and associated with the client ID/secret.\n  developer_portal: https://developer.totalexpert.net (credentials are issued and listed under /credentials)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/authentication/total-expert-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Fintech
- CRM
- Marketing Automation
- Mortgage
- Banking
- Lending
- Customer Engagement
---
