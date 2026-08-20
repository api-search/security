---
api_key_in: []
api_specs:
- filename: salesforce-marketing-cloud-assets-api-openapi.yml
  format: yaml
  label: Salesforce Marketing Cloud Assets API
  slug: salesforce-marketing-cloud-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-marketing-cloud/refs/heads/main/openapi/salesforce-marketing-cloud-assets-api-openapi.yml
- filename: salesforce-marketing-cloud-contacts-api-openapi.yml
  format: yaml
  label: Salesforce Marketing Cloud Contacts API
  slug: salesforce-marketing-cloud-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-marketing-cloud/refs/heads/main/openapi/salesforce-marketing-cloud-contacts-api-openapi.yml
- filename: salesforce-marketing-cloud-journeys-api-openapi.yml
  format: yaml
  label: Salesforce Marketing Cloud Journeys API
  slug: salesforce-marketing-cloud-journeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-marketing-cloud/refs/heads/main/openapi/salesforce-marketing-cloud-journeys-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Salesforce Marketing Cloud Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Salesforce Marketing Cloud secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Salesforce Marketing Cloud
provider_slug: salesforce-marketing-cloud
scheme_count: 1
schemes:
- description: Marketing Cloud Engagement uses OAuth 2.0. Credentials come from an API Integration inside an Installed Package created in Marketing Cloud Setup > Apps > Installed Packages. The Installed Package also fixes which scopes the integration may ever hold.
  flows:
  - docs: https://developer.salesforce.com/docs/marketing/marketing-cloud/guide/access-token-s2s.html
    flow: clientCredentials
    integration_type: Server-to-Server
    scopes: 0
    tokenUrl: https://{subdomain}.auth.marketingcloudapis.com/v2/token
  - docs: https://developer.salesforce.com/docs/marketing/marketing-cloud/guide/integration-considerations.html
    flow: authorizationCode
    integration_type: Web and Public App
    note: '''Web and Public App Integrations with Authorization Code Grant Type.'' Declared in the docs but NOT declared in any captured OpenAPI, which only models clientCredentials.'
    tokenUrl: https://{subdomain}.auth.marketingcloudapis.com/v2/token
  name: OAuth2
  sources:
  - openapi/salesforce-marketing-cloud-assets-api-openapi.yml
  - openapi/salesforce-marketing-cloud-contacts-api-openapi.yml
  - openapi/salesforce-marketing-cloud-journeys-api-openapi.yml
  type: oauth2
slug: salesforce-marketing-cloud-authentication
source_filename: salesforce-marketing-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/salesforce-marketing-cloud-*-openapi.yml (derived baseline)\ndocs:\n  overview: https://developer.salesforce.com/docs/marketing/marketing-cloud/guide/authentication.html\n  integration_types: https://developer.salesforce.com/docs/marketing/marketing-cloud/guide/integration-considerations.html\n  server_to_server: https://developer.salesforce.com/docs/marketing/marketing-cloud/guide/access-token-s2s.html\n  scopes: >-\n    https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\nnote: >-\n  Upgraded from derived to searched on 2026-08-13. The captured OpenAPI declares only the\n  clientCredentials flow; Salesforce's docs additionally document an authorization code flow\n  for web and public apps, plus the token-response fields that make this API workable — most\n  importantly rest_instance_url and soap_instance_url, which are how a client\
  \ discovers its\n  own tenant hosts. A client that hardcodes a subdomain instead of reading these is doing it\n  wrong.\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials, authorizationCode]\n  api_key_in: []\n  mutual_tls: false\n  openid_connect: false\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{subdomain}.auth.marketingcloudapis.com/v2/token\n    scopes: 0\n    integration_type: Server-to-Server\n    docs: https://developer.salesforce.com/docs/marketing/marketing-cloud/guide/access-token-s2s.html\n  - flow: authorizationCode\n    tokenUrl: https://{subdomain}.auth.marketingcloudapis.com/v2/token\n    integration_type: Web and Public App\n    docs: https://developer.salesforce.com/docs/marketing/marketing-cloud/guide/integration-considerations.html\n    note: >-\n      'Web and Public App Integrations with Authorization Code Grant Type.' Declared in the\n      docs but NOT declared in any captured OpenAPI, which\
  \ only models clientCredentials.\n  description: >-\n    Marketing Cloud Engagement uses OAuth 2.0. Credentials come from an API Integration\n    inside an Installed Package created in Marketing Cloud Setup > Apps > Installed Packages.\n    The Installed Package also fixes which scopes the integration may ever hold.\n  sources:\n  - openapi/salesforce-marketing-cloud-assets-api-openapi.yml\n  - openapi/salesforce-marketing-cloud-contacts-api-openapi.yml\n  - openapi/salesforce-marketing-cloud-journeys-api-openapi.yml\ntoken_request:\n  method: POST\n  path: /v2/token\n  host: 'https://{subdomain}.auth.marketingcloudapis.com'\n  fields:\n  - {name: grant_type, required: true, value: client_credentials}\n  - {name: client_id, required: true}\n  - {name: client_secret, required: true}\n  - {name: scope, required: false, description: Space-separated permissions list.}\n  - {name: account_id, required: false, description: 'Business unit MID. \"For server-to-server integrations that use the\
  \ client credentials flow, specify the MID in the account_id parameter of your v2/token request.\"'}\ntoken_response:\n  fields:\n  - {name: access_token, description: 'Acts as a session ID that the application uses to make requests. Max 512 characters.'}\n  - {name: token_type, value: Bearer}\n  - {name: expires_in, value: 1080, description: '\"The value has the value 1080, representing 1,080 seconds, or 18 minutes.\" The real token lifetime is 20 minutes; expires_in is deliberately reported short so a client refreshes before expiry.'}\n  - {name: rest_instance_url, description: The REST API base URL for this tenant. Use this rather than constructing the host.}\n  - {name: soap_instance_url, description: The SOAP API base URL for this tenant.}\n  - {name: scope, description: The permission values actually assigned to the token.}\nrequest_header: 'Authorization: Bearer <access_token>'\ntenancy:\n  subdomain_required: true\n  subdomain_source: Marketing Cloud Setup > Apps > Installed Packages\n\
  \  note: >-\n    Auth, REST and SOAP each live on a different tenant host\n    ({subdomain}.auth / .rest / .soap .marketingcloudapis.com). There is no global host.\nauthorization_model:\n  scope_grant: installed-package\n  runtime_scope_request: false\n  note: >-\n    Scopes are assigned to the Installed Package by an administrator and are fixed for that\n    integration. The scope parameter on the token request can only narrow what the package\n    already holds; it cannot request anything new. A 403 with an errorcode in the 20000 class\n    is therefore an administrative problem, not a client one — it cannot be resolved in code.\n  artifact: scopes/salesforce-marketing-cloud-scopes.yml\nmcp_authentication:\n  differs: true\n  model: OAuth 2.0 authorization code with PKCE (S256), dynamic client registration\n  note: >-\n    The MCE MCP server does NOT use the marketingcloudapis.com auth host. It runs its own\n    authorization server with RFC 8414 metadata, an RFC 7591 registration endpoint\
  \ and PKCE.\n    See mcp/salesforce-marketing-cloud-mcp.yml and\n    well-known/salesforce-marketing-cloud-oauth-authorization-server.json.\nlegacy:\n  v1_endpoint: https://{subdomain}.auth.marketingcloudapis.com/v1/requestToken\n  status: superseded\n  note: The legacy ExactTarget token service. New integrations use v2.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce-marketing-cloud/refs/heads/main/authentication/salesforce-marketing-cloud-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Automation
- Content Management
- Customer Journey
- Digital Marketing
- Email
- Marketing
- Marketing Automation
- MCP
- Mobile Messaging
- Personalization
- SMS
- Webhook
---
