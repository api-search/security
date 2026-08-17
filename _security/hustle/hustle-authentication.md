---
api_key_in: []
api_specs:
- filename: hustle-access-token-api-openapi.yml
  format: yaml
  label: Hustle Access Token API
  slug: hustle-access-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hustle/refs/heads/main/openapi/hustle-access-token-api-openapi.yml
- filename: hustle-agents-api-openapi.yml
  format: yaml
  label: Hustle Agents API
  slug: hustle-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hustle/refs/heads/main/openapi/hustle-agents-api-openapi.yml
- filename: hustle-custom-fields-api-openapi.yml
  format: yaml
  label: Hustle Custom Fields API
  slug: hustle-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hustle/refs/heads/main/openapi/hustle-custom-fields-api-openapi.yml
- filename: hustle-groups-api-openapi.yml
  format: yaml
  label: Hustle Groups API
  slug: hustle-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hustle/refs/heads/main/openapi/hustle-groups-api-openapi.yml
- filename: hustle-integrations-api-openapi.yml
  format: yaml
  label: Hustle Integrations API
  slug: hustle-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hustle/refs/heads/main/openapi/hustle-integrations-api-openapi.yml
- filename: hustle-leads-api-openapi.yml
  format: yaml
  label: Hustle Leads API
  slug: hustle-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hustle/refs/heads/main/openapi/hustle-leads-api-openapi.yml
- filename: hustle-messages-api-openapi.yml
  format: yaml
  label: Hustle Messages API
  slug: hustle-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hustle/refs/heads/main/openapi/hustle-messages-api-openapi.yml
- filename: hustle-organizations-api-openapi.yml
  format: yaml
  label: Hustle Organizations API
  slug: hustle-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hustle/refs/heads/main/openapi/hustle-organizations-api-openapi.yml
- filename: hustle-tags-api-openapi.yml
  format: yaml
  label: Hustle Tags API
  slug: hustle-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hustle/refs/heads/main/openapi/hustle-tags-api-openapi.yml
- filename: hustle-webhooks-api-openapi.yml
  format: yaml
  label: Hustle Webhooks API
  slug: hustle-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hustle/refs/heads/main/openapi/hustle-webhooks-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Hustle Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Hustle secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Hustle
provider_slug: hustle
scheme_count: 1
schemes:
- credentials:
    client_id: email-formatted client id issued by Hustle
    client_secret: secret issued by Hustle
  flow: clientCredentials
  grant_type: client_credentials
  name: OAuth2ClientCredentials
  returns:
    access_token: opaque bearer token
    expires_in: token lifetime in seconds
    scope: returned on the token response
    token_type: Bearer
  sources:
  - openapi/hustle-openapi-original.json
  token_url: https://api.hustle.com/v3/oauth/token
  type: oauth2
  usage: 'Server-side / backend applications authenticate to mint an access token, then send it on subsequent requests as `Authorization: Bearer <token>`.'
slug: hustle-authentication
source_filename: hustle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.hustle.com/v3/docs/\ndocs: https://api.hustle.com/v3/docs/\nspec: openapi/hustle-openapi-original.json\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  token_type: Bearer\n  note: >-\n    The OpenAPI does not declare a components.securitySchemes block; the auth\n    model below is captured from the documented /oauth/token operation and the\n    Bearer authorization described in the spec's response text.\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://api.hustle.com/v3/oauth/token\n  grant_type: client_credentials\n  credentials:\n    client_id: email-formatted client id issued by Hustle\n    client_secret: secret issued by Hustle\n  returns:\n    access_token: opaque bearer token\n    token_type: Bearer\n    scope: returned on the token response\n    expires_in: token lifetime in seconds\n  usage: >-\n    Server-side / backend applications\
  \ authenticate to mint an access token,\n    then send it on subsequent requests as `Authorization: Bearer <token>`.\n  sources: [openapi/hustle-openapi-original.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hustle/refs/heads/main/authentication/hustle-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Enterprise
- Messaging
- SMS
- Peer-to-Peer Texting
- Communications
- Marketing
- Civic Engagement
- Webhooks
- OAuth
---
