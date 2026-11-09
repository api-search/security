---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: jotform-folder-api-openapi.yml
  format: yaml
  label: Jotform Folder API
  slug: jotform-folder-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jotform/openapi/jotform-folder-api-openapi.yml
- filename: jotform-form-api-openapi.yml
  format: yaml
  label: Jotform Form API
  slug: jotform-form-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jotform/openapi/jotform-form-api-openapi.yml
- filename: jotform-label-api-openapi.yml
  format: yaml
  label: Jotform Label API
  slug: jotform-label-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jotform/openapi/jotform-label-api-openapi.yml
- filename: jotform-report-api-openapi.yml
  format: yaml
  label: Jotform Report API
  slug: jotform-report-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jotform/openapi/jotform-report-api-openapi.yml
- filename: jotform-submission-api-openapi.yml
  format: yaml
  label: Jotform Submission API
  slug: jotform-submission-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jotform/openapi/jotform-submission-api-openapi.yml
- filename: jotform-system-api-openapi.yml
  format: yaml
  label: Jotform System API
  slug: jotform-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jotform/openapi/jotform-system-api-openapi.yml
- filename: jotform-user-api-openapi.yml
  format: yaml
  label: Jotform User API
  slug: jotform-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jotform/openapi/jotform-user-api-openapi.yml
- filename: jotform-webhook-api-openapi.yml
  format: yaml
  label: Jotform Webhook API
  slug: jotform-webhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jotform/openapi/jotform-webhook-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Jotform Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jotform secures its APIs with apiKey and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Jotform
provider_slug: jotform
scheme_count: 4
schemes:
- docs: https://api.jotform.com/docs/#authentication
  evidence: 'curl -H "APIKEY: {myApiKey}" "https://api.jotform.com/user"'
  in: header
  key_issuance: My Account -> API Section -> Create a new API Key
  name: ApiKeyHeader
  parameter: APIKEY
  sources:
  - https://api.jotform.com/docs/
  - openapi/jotform-user-api-openapi.yml
  type: apiKey
- docs: https://api.jotform.com/docs/#authentication
  evidence: curl -X GET "https://api.jotform.com/user?apiKey={myApiKey}"
  in: query
  name: ApiKeyQuery
  parameter: apiKey
  sources:
  - https://api.jotform.com/docs/
  - openapi/jotform-user-api-openapi.yml
  type: apiKey
- docs: https://www.jotform.com/developers/tools/
  evidence: 'JF.initialize({ accessType: "readOnly" | "full" }); JF.login(success, error); JF.getAPIKey()'
  in: browser
  name: JavascriptSdkLogin
  note: https://js.jotform.com/JotForm.min.js launches a Jotform login in an iframe and hands the app a user API key with readOnly or full access.
  parameter: null
  sources:
  - https://www.jotform.com/developers/tools/
  - https://api.jotform.com/docs/#authentication
  type: sdk-login
- applies_to: https://mcp.jotform.com and its product servers only
  authorizationUrl: https://oauth2.jotform.com/authorize
  docs: https://www.jotform.com/developers/mcp/?tab=mcp
  evidence: 'Authentication: OAuth 2.0 authorization code flow with PKCE (S256). Each user approves access once on the Jotform consent screen. Jotform API keys are not accepted.'
  flow: authorizationCode
  name: MCPOAuth2
  pkce: S256
  registrationUrl: https://oauth2.jotform.com/register-public-client
  revocationUrl: https://oauth2.jotform.com/revoke
  scopes:
    full: full access (scope name as published)
    readOnly: read access to the user's Jotform data (scope name as published)
  sources:
  - https://www.jotform.com/developers/mcp/?tab=mcp
  - https://mcp.jotform.com/.well-known/oauth-authorization-server
  - https://mcp.jotform.com/.well-known/oauth-protected-resource
  tokenUrl: https://oauth2.jotform.com/token
  type: oauth2
slug: jotform-authentication
source_filename: jotform-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource:\n- https://api.jotform.com/docs/#authentication\n- https://www.jotform.com/developers/tools/\n- https://www.jotform.com/developers/mcp/?tab=mcp\n- https://mcp.jotform.com/.well-known/oauth-authorization-server\ndocs: https://api.jotform.com/docs/#authentication\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  - query\n  statement: 'The Jotform API supports more than one authentication method: the API key as the apiKey query parameter,\n    the API key as the APIKEY HTTP header, or the JavaScript SDK (JF.login) which obtains a key on the user''s behalf\n    with accessType readOnly or full. The MCP server uses OAuth 2.0 only.'\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: APIKEY\n  docs: https://api.jotform.com/docs/#authentication\n  evidence: 'curl -H \"APIKEY: {myApiKey}\" \"https://api.jotform.com/user\"'\n  key_issuance: My Account -> API Section -> Create a new API\
  \ Key\n  sources:\n  - https://api.jotform.com/docs/\n  - openapi/jotform-user-api-openapi.yml\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: apiKey\n  docs: https://api.jotform.com/docs/#authentication\n  evidence: curl -X GET \"https://api.jotform.com/user?apiKey={myApiKey}\"\n  sources:\n  - https://api.jotform.com/docs/\n  - openapi/jotform-user-api-openapi.yml\n- name: JavascriptSdkLogin\n  type: sdk-login\n  in: browser\n  parameter: null\n  docs: https://www.jotform.com/developers/tools/\n  evidence: 'JF.initialize({ accessType: \"readOnly\" | \"full\" }); JF.login(success, error); JF.getAPIKey()'\n  note: https://js.jotform.com/JotForm.min.js launches a Jotform login in an iframe and hands the app a user API\n    key with readOnly or full access.\n  sources:\n  - https://www.jotform.com/developers/tools/\n  - https://api.jotform.com/docs/#authentication\n- name: MCPOAuth2\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://oauth2.jotform.com/authorize\n\
  \  tokenUrl: https://oauth2.jotform.com/token\n  revocationUrl: https://oauth2.jotform.com/revoke\n  registrationUrl: https://oauth2.jotform.com/register-public-client\n  pkce: S256\n  scopes:\n    readOnly: read access to the user's Jotform data (scope name as published)\n    full: full access (scope name as published)\n  applies_to: https://mcp.jotform.com and its product servers only\n  docs: https://www.jotform.com/developers/mcp/?tab=mcp\n  evidence: 'Authentication: OAuth 2.0 authorization code flow with PKCE (S256). Each user approves access once\n    on the Jotform consent screen. Jotform API keys are not accepted.'\n  sources:\n  - https://www.jotform.com/developers/mcp/?tab=mcp\n  - https://mcp.jotform.com/.well-known/oauth-authorization-server\n  - https://mcp.jotform.com/.well-known/oauth-protected-resource\nenterprise_note: Upgrade to Enterprise to make your API url your-domain.com/API or subdomain.jotform.com/API instead\n  of api.jotform.com (api.jotform.com/docs).\n"
source_yaml_url: https://artifacts.apis.io/jotform/authentication/jotform-authentication.yml
summary_line: apiKey/oauth2 · 4 schemes
tags:
- Forms
- Surveys
- No-Code
- Data Collection
- Workflows
- HIPAA
- EU
- MCP
- E-Signature
- Webhook
- Online Payments
---
