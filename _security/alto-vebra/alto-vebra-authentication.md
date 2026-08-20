---
api_key_in:
- header
api_specs:
- filename: alto-api-openapi.json
  format: json
  label: Alto API
  slug: alto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alto-vebra/refs/heads/main/openapi/alto-api-openapi.json
- filename: zoopla-leads-api-openapi.json
  format: json
  label: Zoopla Leads API
  slug: zoopla-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alto-vebra/refs/heads/main/openapi/zoopla-leads-api-openapi.json
- filename: zoopla-premium-listing-activations-openapi.json
  format: json
  label: Zoopla Premium Listing Activations API
  slug: zoopla-premium-listing-activations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alto-vebra/refs/heads/main/openapi/zoopla-premium-listing-activations-openapi.json
- filename: zoopla-weekly-featured-property-openapi.json
  format: json
  label: Zoopla Weekly Featured Property (WFP) Activations API
  slug: zoopla-weekly-featured-property-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alto-vebra/refs/heads/main/openapi/zoopla-weekly-featured-property-openapi.json
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Alto Vebra Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Alto (Vebra / Zoopla) secures its APIs with apiKey and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Alto (Vebra / Zoopla)
provider_slug: alto-vebra
scheme_count: 5
schemes:
- applied: global security requirement on the Alto API
  description: Declared in the Alto OpenAPI as an apiKey-in-header scheme with the description "Please enter JWT with Bearer into field" — an OpenAPI modelling shortcut. The real mechanism is an OAuth 2.0 client-credentials Bearer JWT (see the alto-token scheme below); the spec does not model the token endpoint.
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/alto-api-openapi.json
  type: apiKey
- description: 'Not declared in the OpenAPI; documented in prose at https://developers.vebraalto.com/guides/authenticating-your-requests/. Base64-encode "clientId:clientSecret", send it as an HTTP Basic Authorization header to the token endpoint with Content-Type application/x-www-form-urlencoded and body grant_type=client_credentials. The returned token is presented as "Authorization: Bearer <token>".'
  documented_only: true
  flows:
  - client_authentication: client_secret_basic
    flow: clientCredentials
    note: The documented token endpoint is on the SANDBOX host. The production equivalent (https://api.alto.zoopla.co.uk/token) returns 404 to an anonymous probe. Scopes are published in operation description prose, not in a securitySchemes flow object.
    scopes: 101
    scopes_artifact: scopes/alto-vebra-scopes.yml
    tokenUrl: https://api.alto.zoopladev.co.uk/token
  name: alto-token
  sources:
  - https://developers.vebraalto.com/guides/authenticating-your-requests/
  type: oauth2
- applied: declared as a header parameter on 110 of the 112 Alto operations
  description: Per-agency tenant selector required on every Alto call alongside the Bearer token. Issued to the partner by email when an individual agency activates the integration (https://developers.vebraalto.com/guides/activation-request-emails/). A missing or incorrect AgencyRef yields 403, not 401 — see errors/alto-vebra-problem-types.yml.
  in: header
  name: AgencyRef
  parameter: AgencyRef
  role: tenancy
  sources:
  - openapi/alto-api-openapi.json
  - https://developers.vebraalto.com/guides/error-codes/
  type: apiKey
- flows:
  - audience: https://services.zoopla.co.uk
    client_authentication: client_secret_basic
    flow: clientCredentials
    note: The Leads spec documents an additional `audience` form parameter on the token request.
    scopes: 2
    tokenUrl: https://services-auth.services.zoopla.co.uk/oauth2/token
  name: OAuth2
  sources:
  - openapi/zoopla-leads-api-openapi.json
  type: oauth2
- description: This API uses OAuth 2 with the client credentials grant flow.
  flows:
  - client_authentication: client_secret_basic
    flow: clientCredentials
    scopes: 1
    tokenUrl: https://services-auth.services.zoopla.co.uk/oauth2/token
  name: oAuthSample
  sources:
  - openapi/zoopla-premium-listing-activations-openapi.json
  - openapi/zoopla-weekly-featured-property-openapi.json
  type: oauth2
slug: alto-vebra-authentication
source_filename: alto-vebra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: openapi/alto-api-openapi.json, openapi/zoopla-leads-api-openapi.json, openapi/zoopla-premium-listing-activations-openapi.json,\n  openapi/zoopla-weekly-featured-property-openapi.json\ndocs:\n- https://developers.vebraalto.com/guides/authenticating-your-requests/\n- https://developers.zoopla.co.uk/docs/authentication\n- https://developers.zoopla.co.uk/leads/docs/push-service\n- https://developers.vebraalto.com/guides/webhooks/\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\n  model: >-\n    Two independent OAuth 2.0 client-credentials estates behind one company. Alto issues a Bearer\n    JWT from a /token endpoint on the API host itself; Zoopla issues one from a separate\n    authorization server at services-auth.services.zoopla.co.uk. Neither is self-serve: Alto\n    credentials require an integration registered in Alto Connect under an existing Vebra\n    Solutions\
  \ contract, and Zoopla ships the client_secret PGP-encrypted to a public key the\n    partner supplies out of band. Alto adds a second, non-OAuth authorization dimension — the\n    AgencyRef header — which is the real multi-tenant boundary and is issued per activating\n    agency by email.\n  credential_delivery: out-of-band (email); the Zoopla client_secret is PGP-encrypted to a key\n    the partner exports and hands over\n  self_serve: false\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: >-\n    Declared in the Alto OpenAPI as an apiKey-in-header scheme with the description \"Please\n    enter JWT with Bearer into field\" — an OpenAPI modelling shortcut. The real mechanism is an\n    OAuth 2.0 client-credentials Bearer JWT (see the alto-token scheme below); the spec does not\n    model the token endpoint.\n  applied: global security requirement on the Alto API\n  sources:\n  - openapi/alto-api-openapi.json\n- name: alto-token\n  type:\
  \ oauth2\n  documented_only: true\n  description: >-\n    Not declared in the OpenAPI; documented in prose at\n    https://developers.vebraalto.com/guides/authenticating-your-requests/. Base64-encode\n    \"clientId:clientSecret\", send it as an HTTP Basic Authorization header to the token endpoint\n    with Content-Type application/x-www-form-urlencoded and body grant_type=client_credentials.\n    The returned token is presented as \"Authorization: Bearer <token>\".\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.alto.zoopladev.co.uk/token\n    client_authentication: client_secret_basic\n    scopes: 101\n    scopes_artifact: scopes/alto-vebra-scopes.yml\n    note: >-\n      The documented token endpoint is on the SANDBOX host. The production equivalent\n      (https://api.alto.zoopla.co.uk/token) returns 404 to an anonymous probe. Scopes are\n      published in operation description prose, not in a securitySchemes flow object.\n  sources:\n  - https://developers.vebraalto.com/guides/authenticating-your-requests/\n\
  - name: AgencyRef\n  type: apiKey\n  in: header\n  parameter: AgencyRef\n  role: tenancy\n  description: >-\n    Per-agency tenant selector required on every Alto call alongside the Bearer token. Issued to\n    the partner by email when an individual agency activates the integration\n    (https://developers.vebraalto.com/guides/activation-request-emails/). A missing or incorrect\n    AgencyRef yields 403, not 401 — see errors/alto-vebra-problem-types.yml.\n  applied: declared as a header parameter on 110 of the 112 Alto operations\n  sources:\n  - openapi/alto-api-openapi.json\n  - https://developers.vebraalto.com/guides/error-codes/\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://services-auth.services.zoopla.co.uk/oauth2/token\n    client_authentication: client_secret_basic\n    scopes: 2\n    audience: https://services.zoopla.co.uk\n    note: The Leads spec documents an additional `audience` form parameter on the token request.\n  sources:\n\
  \  - openapi/zoopla-leads-api-openapi.json\n- name: oAuthSample\n  type: oauth2\n  description: This API uses OAuth 2 with the client credentials grant flow.\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://services-auth.services.zoopla.co.uk/oauth2/token\n    client_authentication: client_secret_basic\n    scopes: 1\n  sources:\n  - openapi/zoopla-premium-listing-activations-openapi.json\n  - openapi/zoopla-weekly-featured-property-openapi.json\nidentity_provider:\n  host: https://id.vebraalto.com\n  vendor: Auth0\n  role: Alto Connect / Developer Portal human login (NOT the API token issuer)\n  discovery: well-known/alto-vebra-openid-configuration.json\n  grant_types_supported:\n  - client_credentials\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  dpop_supported: true\ninbound_callback_auth:\n  description: >-\n    Alto authenticates\
  \ ITSELF to the partner when delivering webhooks; the partner chooses the\n    method during onboarding. Documented at https://developers.vebraalto.com/guides/webhooks/.\n  methods:\n  - type: apiKey\n    header: x-signature\n    description: Shared secret presented by Alto on each callback.\n  - type: http\n    scheme: basic\n    description: HTTP Basic username/password issued to Alto during onboarding.\n  - type: oauth2\n    flow: clientCredentials\n    description: Alto obtains a bearer token from the partner's own authorization server.\n  zoopla_push:\n    docs: https://developers.zoopla.co.uk/leads/docs/push-service\n    methods:\n    - type: oauth2\n      flow: clientCredentials\n      description: Zoopla calls a token endpoint the partner supplies, then sends Authorization\n        Bearer.\n    - type: apiKey\n      header: Authorization\n      description: Key used verbatim as the Authorization header value.\ngaps:\n- No mutualTLS, no openIdConnect scheme and no PKCE anywhere\
  \ on the API surface — every path is\n  machine-to-machine client credentials.\n- Neither the Alto nor the Zoopla token endpoint publishes RFC 8414 metadata; the only discovery\n  document in the estate belongs to the human-login Auth0 tenant.\n- The Alto OpenAPI models the Bearer JWT as an apiKey scheme, so generated clients will not know\n  a token endpoint exists.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alto-vebra/refs/heads/main/authentication/alto-vebra-authentication.yml
summary_line: apiKey/oauth2 · 5 schemes
tags:
- Real-Estate
- United Kingdom
- PropTech
- Property Listings
- CRM
- Property Management
- Rentals
- Conveyancing
- Estate Agency
- Tenancy
- Webhook
- Event
- Lettings
- Sales Progression
- Property Data
- Real Estate Software
---
