---
api_key_in: []
auth_types: []
description: 'RainFocus publishes no OpenAPI, so no securityScheme block could be derived. This profile is assembled from three things that ARE public: the OIDC/OAuth discovery documents RainFocus serves itself, the live behaviour of api.rainfocus.com and its MCP endpoint under an unauthenticated request, and the RainFocus-authored setup instructions carried in the Adobe Experience Platform destination connector. Nothing here is invented and no credential values appear.'
kind: authentication
layout: security
method: searched
name: Rainfocus Authentication
name_suffix: Authentication
oauth_flows: []
overview: RainFocus declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: RainFocus
provider_slug: rainfocus
scheme_count: 4
schemes:
- companion_headers:
  - rfApiProfileId
  - authToken
  - rfAuthToken
  - rfWidgetId
  - widget
  - rfcsrf
  - extraFields
  companion_headers_note: Observed in the Access-Control-Allow-Headers response header on api.rainfocus.com. Their individual semantics are not publicly documented and are not guessed at here.
  description: 'Every request to a /api path on api.rainfocus.com must name an API Profile. An API Profile is a named integration configuration created per customer in the RainFocus Integration Suite that declares which endpoints are enabled (for example Attendee Store) and carries the modular field mappings for that integration. Omitting it returns HTTP 400 with responseCode 103 and "Required parameter missing: apiProfile".'
  evidence:
    body: '{"responseCode":"103","responseMessage":"Required parameter missing: apiProfile"}'
    request: GET https://api.rainfocus.com/api
    status: 400
  id: api-profile
  in: header
  name: apiProfile
  required: true
  type: apiKey
- description: 'RainFocus API Profiles can be created with "OAuth (Global)", which issues a Client ID and Client Secret used by server-to-server integrations. This is the credential model the Adobe Experience Platform RainFocus destination requires: "Create a RainFocus API Profile with OAuth (Global)", ensure the Attendee Store endpoint is enabled, and generate a Client ID and Client Secret.'
  flow: client_credentials
  id: oauth2-global
  parameters_required_by_integrators:
  - example_values:
    - dev
    - prod
    name: environment
  - name: orgId
    note: unique organization identifier for the customer's RainFocus instance
  - name: eventId
    note: RainFocus event code identifying the destination event
  source: https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/marketing-automation/rainfocus - a connector page RainFocus itself authors and maintains.
  token_endpoint: null
  token_endpoint_note: Not published. The customer-facing token URL is delivered with the profile credentials, not on the public web.
  type: oauth2
- authorization_endpoint: https://events.rainfocus.com/oidc/auth
  description: A full OpenID Connect provider fronted by both api.rainfocus.com and events.rainfocus.com. This is the authorization server the MCP endpoint delegates to.
  grant_types_supported:
  - authorization_code
  - refresh_token
  id: oidc
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://events.rainfocus.com/oidc
  jwks_uri: https://events.rainfocus.com/oidc/.well-known/jwks
  openIdConnectUrl: https://api.rainfocus.com/.well-known/openid-configuration
  pkce_note: code_challenge_methods_supported is absent from the discovery document, so PKCE support is not advertised. That is a real gap for a public MCP client.
  pkce_supported: false
  response_modes_supported:
  - query
  response_types_supported:
  - code
  - id_token
  - token
  - code id_token
  - code token
  - id_token token
  - code id_token token
  scopes_supported:
  - openid
  subject_types_supported:
  - public
  token_endpoint: https://events.rainfocus.com/oidc/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
  userinfo_endpoint: https://events.rainfocus.com/oidc/userData
- applies_to: https://api.rainfocus.com/mcp/
  authorization_servers:
  - https://events.rainfocus.com/oidc
  bearer_token_methods_supported:
  - header
  description: The RainFocus Nexus MCP endpoint requires an OAuth bearer token in the Authorization header. An unauthenticated tools/list POST returns 401 with a WWW-Authenticate challenge naming RFC 9728 protected-resource metadata, which is the discovery path an MCP client follows to find the authorization server.
  evidence:
    request: POST https://api.rainfocus.com/mcp/ tools/list
    status: 401
    www_authenticate: Bearer resource_metadata="https://events.rainfocus.com/.well-known/oauth-protected-resource/mcp//"
  id: mcp-bearer
  scheme: bearer
  token_lifetime: RainFocus describes short-lived, scoped access tokens plus refresh tokens with per-user authentication, role-based access control and per-event scoping.
  type: http
slug: rainfocus-authentication
source_filename: rainfocus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: >-\n  https://api.rainfocus.com/.well-known/openid-configuration (probed) +\n  https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/marketing-automation/rainfocus\n  (RainFocus-authored connector documentation) +\n  https://www.rainfocus.com/privacy-security/api-terms-and-conditions/\ndocs: https://www.rainfocus.com/privacy-security/api-terms-and-conditions/\ndescription: >-\n  RainFocus publishes no OpenAPI, so no securityScheme block could be derived. This profile is\n  assembled from three things that ARE public: the OIDC/OAuth discovery documents RainFocus serves\n  itself, the live behaviour of api.rainfocus.com and its MCP endpoint under an unauthenticated\n  request, and the RainFocus-authored setup instructions carried in the Adobe Experience Platform\n  destination connector. Nothing here is invented and no credential values appear.\nderivation_note: >-\n  derive-authentication.py was\
  \ not run - it reads openapi/ securitySchemes and this repo has no\n  spec. Everything below is probed or read from published documentation.\nschemes:\n- id: api-profile\n  type: apiKey\n  in: header\n  name: apiProfile\n  required: true\n  description: >-\n    Every request to a /api path on api.rainfocus.com must name an API Profile. An API Profile is a\n    named integration configuration created per customer in the RainFocus Integration Suite that\n    declares which endpoints are enabled (for example Attendee Store) and carries the modular field\n    mappings for that integration. Omitting it returns HTTP 400 with responseCode 103 and\n    \"Required parameter missing: apiProfile\".\n  evidence:\n    request: GET https://api.rainfocus.com/api\n    status: 400\n    body: '{\"responseCode\":\"103\",\"responseMessage\":\"Required parameter missing: apiProfile\"}'\n  companion_headers:\n  - rfApiProfileId\n  - authToken\n  - rfAuthToken\n  - rfWidgetId\n  - widget\n  - rfcsrf\n  - extraFields\n\
  \  companion_headers_note: >-\n    Observed in the Access-Control-Allow-Headers response header on api.rainfocus.com. Their\n    individual semantics are not publicly documented and are not guessed at here.\n- id: oauth2-global\n  type: oauth2\n  flow: client_credentials\n  description: >-\n    RainFocus API Profiles can be created with \"OAuth (Global)\", which issues a Client ID and\n    Client Secret used by server-to-server integrations. This is the credential model the Adobe\n    Experience Platform RainFocus destination requires: \"Create a RainFocus API Profile with OAuth\n    (Global)\", ensure the Attendee Store endpoint is enabled, and generate a Client ID and Client\n    Secret.\n  parameters_required_by_integrators:\n  - name: environment\n    example_values: [dev, prod]\n  - name: orgId\n    note: unique organization identifier for the customer's RainFocus instance\n  - name: eventId\n    note: RainFocus event code identifying the destination event\n  token_endpoint: null\n\
  \  token_endpoint_note: >-\n    Not published. The customer-facing token URL is delivered with the profile credentials, not on\n    the public web.\n  source: >-\n    https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/marketing-automation/rainfocus\n    - a connector page RainFocus itself authors and maintains.\n- id: oidc\n  type: openIdConnect\n  openIdConnectUrl: https://api.rainfocus.com/.well-known/openid-configuration\n  issuer: https://events.rainfocus.com/oidc\n  description: >-\n    A full OpenID Connect provider fronted by both api.rainfocus.com and events.rainfocus.com. This\n    is the authorization server the MCP endpoint delegates to.\n  authorization_endpoint: https://events.rainfocus.com/oidc/auth\n  token_endpoint: https://events.rainfocus.com/oidc/token\n  userinfo_endpoint: https://events.rainfocus.com/oidc/userData\n  jwks_uri: https://events.rainfocus.com/oidc/.well-known/jwks\n  scopes_supported: [openid]\n  response_types_supported:\n\
  \  - code\n  - id_token\n  - token\n  - code id_token\n  - code token\n  - id_token token\n  - code id_token token\n  response_modes_supported: [query]\n  grant_types_supported: [authorization_code, refresh_token]\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post]\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [public]\n  pkce_supported: false\n  pkce_note: >-\n    code_challenge_methods_supported is absent from the discovery document, so PKCE support is not\n    advertised. That is a real gap for a public MCP client.\n- id: mcp-bearer\n  type: http\n  scheme: bearer\n  description: >-\n    The RainFocus Nexus MCP endpoint requires an OAuth bearer token in the Authorization header. An\n    unauthenticated tools/list POST returns 401 with a WWW-Authenticate challenge naming RFC 9728\n    protected-resource metadata, which is the discovery path an MCP client follows to find the\n    authorization server.\n  applies_to: https://api.rainfocus.com/mcp/\n\
  \  bearer_token_methods_supported: [header]\n  authorization_servers: [https://events.rainfocus.com/oidc]\n  token_lifetime: >-\n    RainFocus describes short-lived, scoped access tokens plus refresh tokens with per-user\n    authentication, role-based access control and per-event scoping.\n  evidence:\n    request: POST https://api.rainfocus.com/mcp/ tools/list\n    status: 401\n    www_authenticate: Bearer resource_metadata=\"https://events.rainfocus.com/.well-known/oauth-protected-resource/mcp//\"\ncredential_handling_obligations:\n  source: https://www.rainfocus.com/privacy-security/api-terms-and-conditions/\n  obligations:\n  - Customer must maintain the confidentiality of all API keys, MCP credentials, tokens and endpoints.\n  - Sharing, distributing or exposing API keys, MCP credentials, tokens or endpoints to any unauthorized person or system is prohibited.\n  - Bypassing or circumventing usage limits, rate limits, authentication or security controls is prohibited.\n  - On termination,\
  \ Customer must destroy all copies of API keys, MCP credentials, tokens and cached API responses.\ngaps:\n- No public authentication reference page; the auth model must be reconstructed from a partner connector doc.\n- No PKCE advertised in OIDC discovery.\n- scopes_supported is only \"openid\" - no resource scopes are published for either the REST API or the MCP server.\n- No token endpoint published for the OAuth (Global) client-credentials flow.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rainfocus/refs/heads/main/authentication/rainfocus-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Events
- Event Management
- Event Marketing
- Registration
- Conferences
- Webinars
- Marketing Technology
- Attendee Data
- MCP
- Agents
- Enterprise Software
- SaaS
---
