---
api_key_in:
- header
- body
api_specs:
- filename: mailchimp-marketing-api-openapi.yml
  format: yaml
  label: Mailchimp Marketing API
  slug: mailchimp-marketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailchimp/refs/heads/main/openapi/mailchimp-marketing-api-openapi.yml
- filename: mailchimp-transactional-api-openapi.yml
  format: yaml
  label: Mailchimp Transactional API
  slug: mailchimp-transactional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailchimp/refs/heads/main/openapi/mailchimp-transactional-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Mailchimp Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Mailchimp secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Mailchimp
provider_slug: mailchimp
scheme_count: 3
schemes:
- api: mailchimp:mailchimp-marketing-api
  description: Marketing API HTTP Basic auth. Use any string as the username and the API key as the password. The API key carries a datacenter suffix (e.g. -us19) which also determines the request host <dc>.api.mailchimp.com.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/mailchimp-marketing-api-openapi.yml
  type: http
- api: mailchimp:mailchimp-marketing-api
  authorizationUrl: https://login.mailchimp.com/oauth2/authorize
  description: OAuth 2.0 authorization-code flow for accessing a user's Mailchimp data (used by apps/integrations). Mailchimp OAuth grants full account access and does NOT use granular scopes. After the token exchange, call the metadata endpoint to discover the account's datacenter (dc) for API requests. Not declared in the OpenAPI securityDefinitions; documented only.
  flow: authorizationCode
  metadataUrl: https://login.mailchimp.com/oauth2/metadata
  name: oauth2
  scopes: []
  sources:
  - https://mailchimp.com/developer/marketing/guides/access-user-data-oauth-2/
  tokenUrl: https://login.mailchimp.com/oauth2/token
  type: oauth2
- api: mailchimp:mailchimp-transactional-api
  description: Transactional (Mandrill) API key authentication. The key is passed in the JSON request body as the "key" parameter for every POST call, or alternatively via the X-MC-ApiKey header. A "test" API key exercises the API in test mode without delivering mail (see sandbox/mailchimp-sandbox.yml).
  in: header
  name: apiKey
  parameter: X-MC-ApiKey
  sources:
  - openapi/mailchimp-transactional-api-openapi.yml
  type: apiKey
slug: mailchimp-authentication
source_filename: mailchimp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: >-\n  openapi/mailchimp-marketing-api-openapi.yml,\n  openapi/mailchimp-transactional-api-openapi.yml, enriched from\n  https://mailchimp.com/developer/marketing/guides/access-user-data-oauth-2/ and\n  https://mailchimp.com/developer/transactional/docs/authentication-delivery/\ndocs:\n  - https://mailchimp.com/developer/marketing/guides/access-user-data-oauth-2/\n  - https://mailchimp.com/developer/transactional/docs/authentication-delivery/\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  - body\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  api: mailchimp:mailchimp-marketing-api\n  description: >-\n    Marketing API HTTP Basic auth. Use any string as the username and the API\n    key as the password. The API key carries a datacenter suffix (e.g. -us19)\n    which also determines the request host <dc>.api.mailchimp.com.\n  sources:\n\
  \  - openapi/mailchimp-marketing-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  api: mailchimp:mailchimp-marketing-api\n  flow: authorizationCode\n  authorizationUrl: https://login.mailchimp.com/oauth2/authorize\n  tokenUrl: https://login.mailchimp.com/oauth2/token\n  metadataUrl: https://login.mailchimp.com/oauth2/metadata\n  scopes: []\n  description: >-\n    OAuth 2.0 authorization-code flow for accessing a user's Mailchimp data\n    (used by apps/integrations). Mailchimp OAuth grants full account access and\n    does NOT use granular scopes. After the token exchange, call the metadata\n    endpoint to discover the account's datacenter (dc) for API requests. Not\n    declared in the OpenAPI securityDefinitions; documented only.\n  sources:\n  - https://mailchimp.com/developer/marketing/guides/access-user-data-oauth-2/\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-MC-ApiKey\n  api: mailchimp:mailchimp-transactional-api\n  description: >-\n    Transactional (Mandrill)\
  \ API key authentication. The key is passed in the\n    JSON request body as the \"key\" parameter for every POST call, or\n    alternatively via the X-MC-ApiKey header. A \"test\" API key exercises the\n    API in test mode without delivering mail (see sandbox/mailchimp-sandbox.yml).\n  sources:\n  - openapi/mailchimp-transactional-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailchimp/refs/heads/main/authentication/mailchimp-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Campaigns
- Email Marketing
- Marketing Automation
- Newsletters
- Transactional Email
---
