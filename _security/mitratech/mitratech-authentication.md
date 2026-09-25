---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mitratech-dashboard-api-openapi.yml
  format: yaml
  label: Mitratech Dashboard API
  slug: mitratech-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mitratech/refs/heads/main/openapi/mitratech-dashboard-api-openapi.yml
- filename: mitratech-files-api-openapi.yml
  format: yaml
  label: Mitratech Files API
  slug: mitratech-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mitratech/refs/heads/main/openapi/mitratech-files-api-openapi.yml
- filename: mitratech-gridconfigurations-api-openapi.yml
  format: yaml
  label: Mitratech Grid Configurations API
  slug: mitratech-gridconfigurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mitratech/refs/heads/main/openapi/mitratech-gridconfigurations-api-openapi.yml
- filename: mitratech-templates-api-openapi.yml
  format: yaml
  label: Mitratech Templates API
  slug: mitratech-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mitratech/refs/heads/main/openapi/mitratech-templates-api-openapi.yml
- filename: mitratech-users-api-openapi.yml
  format: yaml
  label: Mitratech Users API
  slug: mitratech-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mitratech/refs/heads/main/openapi/mitratech-users-api-openapi.yml
- filename: mitratech-workflow-api-openapi.yml
  format: yaml
  label: Mitratech Workflow API
  slug: mitratech-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mitratech/refs/heads/main/openapi/mitratech-workflow-api-openapi.yml
- filename: mitratech-workflows-api-openapi.yml
  format: yaml
  label: Mitratech Workflows API
  slug: mitratech-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mitratech/refs/heads/main/openapi/mitratech-workflows-api-openapi.yml
- filename: mitratech-health-check-api-openapi.yml
  format: yaml
  label: Mitratech Health Check API
  slug: mitratech-health-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mitratech/refs/heads/main/openapi/mitratech-health-check-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Mitratech Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mitratech declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Mitratech
provider_slug: mitratech
scheme_count: 0
schemes: []
slug: mitratech-authentication
source_filename: mitratech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: searched\nsource: >-\n  https://success.mitratech.com/TAP/TAP_Solutions/APIs_and_Integrations/TAP_API_Documentation +\n  https://success.mitratech.com/TeamConnect/TeamConnect_Setup_and_Development/TeamConnect_REST_API_Modernization_(TCE_7.2)/TeamConnect_RESTAPIs_-_Authentication +\n  https://mitratech.com/.well-known/oauth-authorization-server\ndocs:\n- https://success.mitratech.com/TAP/TAP_Solutions/APIs_and_Integrations/TAP_API_Documentation\n- https://success.mitratech.com/TeamConnect/TeamConnect_Setup_and_Development/TeamConnect_REST_API_Modernization_(TCE_7.2)/TeamConnect_RESTAPIs_-_Authentication\nsummary: >-\n  Every Mitratech programmatic surface is OAuth 2.0, but the three surfaces use three different flows\n  and three different token issuers. The harvested TAP Swagger 2.0 document declares NO\n  securityDefinitions at all — the auth model exists only in prose on the Success Center, which is why\n  this artifact is method: searched\
  \ rather than derived from the spec.\napis:\n- api: Mitratech TAP Workflow Automation API\n  schemes:\n  - id: tap_oauth2_password\n    type: oauth2\n    flow: password\n    grant_type: password\n    token_endpoint: https://{tenant}.tap.thinksmart.com/{tenant}/auth/identity/connect/token\n    token_endpoint_staging: https://{tenant}.stagingtap.thinksmart.com/{tenant}/auth/identity/connect/token\n    content_type: application/x-www-form-urlencoded\n    parameters:\n    - name: grant_type\n      value: password\n    - name: scope\n      value: api\n    - name: redirect_uri\n      value: tapredirect\n      note: Typical default value; the docs say to confirm it with Mitratech.\n    - name: username\n      note: The registered TAP user to be authorized.\n    - name: password\n      note: That user's password.\n    - name: client_id\n      note: Obtained from Mitratech — not self-serve.\n    - name: client_secret\n      note: Obtained from Mitratech — not self-serve.\n    token_type: Bearer\n\
  \    expires_in: 3600\n    presentation: 'Authorization: Bearer <access_token>'\n    authorization_model: >-\n      The token inherits the permissions of the TAP user account it was issued for. Mitratech's own\n      documentation warns that a non-Super-Admin account will silently return incomplete result sets\n      rather than a 403 — an authorization pitfall an agent cannot detect from the response.\n    spec_declared: false\n    spec_note: >-\n      openapi/_original/mitratech-tap-swagger.json has no securityDefinitions and no security block on\n      any of its 49 operations. A client generated from the spec alone would send no credentials.\n- api: Mitratech TeamConnect REST API\n  schemes:\n  - id: teamconnect_oauth2_authorization_code\n    type: oauth2\n    flow: authorizationCode\n    authorization_endpoint: https://{your-tc-instance}/webservice/enterprise/oauth/authorize\n    token_endpoint: https://{your-tc-instance}/webservice/enterprise/oauth/token\n    client_authentication:\
  \ Basic auth header\n    token_type: Bearer\n    note: >-\n      Available in TeamConnect Enterprise 7.2 and later only. Backward compatibility with pre-7.2\n      REST APIs was deliberately dropped.\n  - id: teamconnect_oauth2_client_credentials\n    type: oauth2\n    flow: clientCredentials\n    token_endpoint: https://{your-tc-instance}/webservice/enterprise/oauth/token\n    client_authentication: Basic auth header\n    token_type: Bearer\n    note: Server-to-server integrations without a user in the loop.\n  client_registration: >-\n    API clients are registered inside the customer's own TeamConnect instance —\n    Setup > System Settings > API Client Settings — where an admin supplies a Name, Description,\n    Homepage URL and Callback URL and TeamConnect issues an API Client ID. There is no central\n    Mitratech developer console and no self-serve key.\n  token_lifetime:\n    model: rolling idle expiration\n    idle_window_days: 30\n    note: >-\n      Mitratech documents that\
  \ TeamConnect access tokens use a rolling 30-day idle expiration and that\n      each valid use resets the window. It also documents that the `expires_in` value in the token\n      response is a hardcoded server response that clients should IGNORE. This is a real agent hazard:\n      the machine-readable field in the response contradicts the documented behaviour.\n- api: Mitratech MCP Server\n  schemes:\n  - id: mcp_oauth2_authorization_code_pkce\n    type: oauth2\n    flow: authorizationCode\n    issuer: https://mitratech.com\n    authorization_endpoint: https://mitratech.com/oauth/authorize\n    token_endpoint: https://mitratech.com/oauth/token\n    revocation_endpoint: https://mitratech.com/oauth/revoke\n    pkce: S256\n    grant_types: [authorization_code, refresh_token]\n    scopes: [mcp]\n    token_endpoint_auth_methods_supported: [none]\n    client_id_metadata_document_supported: true\n    bearer_methods_supported: [header]\n    discovery:\n    - well-known/mitratech-oauth-authorization-server.json\n\
  \    - well-known/mitratech-oauth-protected-resource.json\n    method: probed\ngaps:\n- No API key or personal-access-token option is documented on any surface.\n- >-\n  TAP's only documented grant is the OAuth 2.0 resource owner password credentials grant, which\n  OAuth 2.1 and RFC 9700 (BCP for OAuth 2.0 Security) both deprecate. It requires the integration to\n  hold a real TAP user's password.\n- >-\n  TAP client_id and client_secret are issued by Mitratech on request, not through self-service, so\n  there is no path from reading the public docs to making an authenticated call.\n- The TAP Swagger document carries no securityDefinitions, so the auth model is not machine-readable.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mitratech/refs/heads/main/authentication/mitratech-authentication.yml
summary_line: 0 schemes
tags:
- Legal
- Legal Operations
- Enterprise Legal Management
- Matter Management
- Governance Risk and Compliance
- Compliance
- Workflow Automation
- Contract Lifecycle Management
- HR Compliance
- Risk Management
- Immigration
- OData
- MCP
---
