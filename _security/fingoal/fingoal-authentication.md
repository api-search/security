---
api_key_in: []
api_specs:
- filename: fingoal-enrichment-api-openapi.yml
  format: yaml
  label: FinGoal Enrichment API
  slug: fingoal-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fingoal/refs/heads/main/openapi/fingoal-enrichment-api-openapi.yml
- filename: fingoal-user-tagging-api-openapi.yml
  format: yaml
  label: FinGoal User Tagging API
  slug: fingoal-user-tagging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fingoal/refs/heads/main/openapi/fingoal-user-tagging-api-openapi.yml
- filename: fingoal-webhook-configurations-api-openapi.yml
  format: yaml
  label: FinGoal Webhook Configurations API
  slug: fingoal-webhook-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fingoal/refs/heads/main/openapi/fingoal-webhook-configurations-api-openapi.yml
- filename: fingoal-client-management-api-openapi.yml
  format: yaml
  label: FinGoal Client Management API
  slug: fingoal-client-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fingoal/refs/heads/main/openapi/fingoal-client-management-api-openapi.yml
- filename: fingoal-fastlink-api-openapi.yml
  format: yaml
  label: FinGoal Fastlink API
  slug: fingoal-fastlink-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fingoal/refs/heads/main/openapi/fingoal-fastlink-api-openapi.yml
- filename: fingoal-oauth-api-openapi.yml
  format: yaml
  label: FinGoal OAUTH API
  slug: fingoal-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fingoal/refs/heads/main/openapi/fingoal-oauth-api-openapi.yml
- filename: fingoal-webhooks-api-openapi.yml
  format: yaml
  label: FinGoal Webhooks API
  slug: fingoal-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fingoal/refs/heads/main/openapi/fingoal-webhooks-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Fingoal Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: FinGoal secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: FinGoal
provider_slug: fingoal
scheme_count: 2
schemes:
- api: fingoal:fingoal-enrichment-api
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://findmoney.fingoal.com/v3/authentication
  name: Authentication
  sources:
  - openapi/fingoal-insights-openapi-original.json
  type: oauth2
- api: fingoal:fingoal-link-money-api
  flows:
  - flow: clientCredentials
    scope_names:
    - tenantId
    scopes: 1
    tokenUrl: https://link-money-dev.fingoal.dev/api/oauth/token
  name: BearerAuth
  notes: 'Link Money declares oauth2 clientCredentials but is not RFC 6749 shaped. POST /api/oauth/token takes a JSON body of CAMEL-cased {clientId, clientSecret, tenantId} and returns {token} - not {access_token, token_type, expires_in}. The single declared "scope" is tenantId, which is really a tenancy selector: the JWT is valid for 1 hour and grants access to exactly one tenant, so multi-tenant integrations must mint one token per tenant. Send it as Authorization: Bearer <token>. Tenant access itself is granted out of band - email support@fingoal.com; clients cannot create tenants.'
  sources:
  - openapi/_original/fingoal-link-money-openapi-original.json
  type: oauth2
slug: fingoal-authentication
source_filename: fingoal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/fingoal-insights-openapi-original.json\ndocs: https://docs.fingoal.dev/\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nnotes: >-\n  The Insights API is declared as OAuth2 clientCredentials in the OpenAPI, but\n  the token is minted by a custom endpoint: POST\n  https://findmoney.fingoal.com/v3/authentication with a JSON body\n  {\"client_id\",\"client_secret\"} returns a JWT `access_token`. That JWT is then\n  sent as `Authorization: Bearer <token>` on every request. Developer\n  credentials are issued on request (24h turnaround) via\n  https://fingoal.com/request-developer-account - there is no public self-serve\n  signup. Dev credentials target the findmoney-dev host; production the\n  findmoney host.\nschemes:\n- name: Authentication\n  type: oauth2\n  api: fingoal:fingoal-enrichment-api\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://findmoney.fingoal.com/v3/authentication\n\
  \    scopes: 1\n  sources:\n  - openapi/fingoal-insights-openapi-original.json\n- name: BearerAuth\n  type: oauth2\n  api: fingoal:fingoal-link-money-api\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://link-money-dev.fingoal.dev/api/oauth/token\n    scopes: 1\n    scope_names:\n    - tenantId\n  sources:\n  - openapi/_original/fingoal-link-money-openapi-original.json\n  notes: >-\n    Link Money declares oauth2 clientCredentials but is not RFC 6749 shaped. POST\n    /api/oauth/token takes a JSON body of CAMEL-cased {clientId, clientSecret,\n    tenantId} and returns {token} - not {access_token, token_type, expires_in}.\n    The single declared \"scope\" is tenantId, which is really a tenancy selector:\n    the JWT is valid for 1 hour and grants access to exactly one tenant, so\n    multi-tenant integrations must mint one token per tenant. Send it as\n    Authorization: Bearer <token>. Tenant access itself is granted out of band -\n    email support@fingoal.com; clients cannot\
  \ create tenants.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fingoal/refs/heads/main/authentication/fingoal-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Financial-Services
- Fintech
- Transaction Enrichment
- Data Enrichment
- Personal Financial Management
- Banking
- Categorization
- Webhook
---
