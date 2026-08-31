---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Sightcall Authentication
name_suffix: Authentication
oauth_flows: []
overview: SightCall declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: SightCall
provider_slug: sightcall
scheme_count: 0
schemes: []
slug: sightcall-authentication
source_filename: sightcall-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: https://docs.sightcall.com/gd/how-to/authenticate (page is now gated - 307 to https://admin.sightcall.com/; detail below is from the publicly indexed version of SightCall's own documentation)\ndocs: https://docs.sightcall.com/gd/how-to/authenticate\nnote: >-\n  SightCall's REST API authentication model is documented on the company's own developer documentation site, which as\n  of 2026-08-27 is no longer publicly reachable: every path under docs.sightcall.com returns HTTP 307 to\n  https://admin.sightcall.com/, the console login. SightCall's own llms.txt confirms the posture - \"Developer Portal:\n  SDK documentation for iOS, Android, and Web. REST API reference and integration guides. (Contact SightCall for\n  access.)\" The scheme recorded here is taken from the publicly indexed text of SightCall's own authenticate and\n  rest-api pages; it is NOT derived from an OpenAPI (none is published) and it could not be re-verified\
  \ against a\n  live document. No OAuth 2.0 or OpenID Connect surface is documented for the REST API, so no scopes/ artifact is\n  written. SAML/OIDC SSO is offered for END-USER console login (per sightcall.com/platform/security/), which is a\n  different surface from API authentication.\nverification:\n  live_docs_reachable: false\n  docs_status: 307\n  redirect_to: https://admin.sightcall.com/\n  openapi_available: false\nsecurity_schemes:\n- id: apiKeyHeader\n  type: apiKey\n  in: header\n  name: Authorization\n  scheme_format: 'Authorization: Apikey <API_KEY>'\n  description: >-\n    Application back ends authenticate to the SightCall REST API with an API key in the Authorization header. The API\n    key is the concatenation of the Authentication API Client Identifier and the Authentication API Client Secret.\n  applies_to: provider/back-end REST methods\n  confidence: medium\n  evidence: SightCall documentation (docs.sightcall.com/gd/how-to/authenticate), publicly indexed; page now\
  \ gated.\n- id: userToken\n  type: apiKey\n  in: header\n  name: Authorization\n  scheme_format: '<appId>/<token>'\n  description: >-\n    Client/user authentication uses a token minted by the back end through the provider REST API. The user credential\n    is the appId and the token joined by a forward slash. Tokens are requested per user UID and domain.\n  applies_to: end-user/client SDK sessions\n  confidence: medium\n  evidence: SightCall documentation (docs.sightcall.com/gd/rest-api, gd/how-to/authenticate), publicly indexed.\nkey_management:\n  where_to_find: SightCall admin console (https://admin.sightcall.com/) - per the SightCall Help Center article \"Where can I find my SightCall API Key?\"\n  rotation_policy: not published\noauth:\n  present: false\n  note: No OAuth 2.0 / OIDC authorization server is documented or discoverable for the SightCall REST API. /.well-known/oauth-authorization-server and /.well-known/openid-configuration miss on every SightCall host (see well-known/sightcall-well-known.yml).\n\
  sso:\n- protocol: SAML\n  scope: console/user sign-in (not API auth)\n  source: https://sightcall.com/platform/security/\n- protocol: OIDC\n  scope: console/user sign-in (not API auth)\n  source: https://sightcall.com/platform/security/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sightcall/refs/heads/main/authentication/sightcall-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Video
- WebRTC
- Remote Support
- Field Service
- Augmented Reality
- Computer-Vision
- Customer Service
- Insurance
- Telehealth
- Communications
---
