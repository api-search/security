---
api_key_in: []
api_specs:
- filename: tremor-video.postman_collection.json
  format: json
  label: Nexxen DSP API
  slug: nexxen-dsp-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/tremor-video/refs/heads/main/collections/tremor-video.postman_collection.json
- filename: tremor-video.postman_collection.json
  format: json
  label: Nexxen DSP Token Service
  slug: nexxen-dsp-token-service
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/tremor-video/refs/heads/main/collections/tremor-video.postman_collection.json
- filename: tremor-video.postman_collection.json
  format: json
  label: Nexxen DSP Reporting API
  slug: nexxen-dsp-reporting-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/tremor-video/refs/heads/main/collections/tremor-video.postman_collection.json
- filename: tremor-video.postman_collection.json
  format: json
  label: Nexxen DSP Device API
  slug: nexxen-dsp-device-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/tremor-video/refs/heads/main/collections/tremor-video.postman_collection.json
- filename: tremor-video.postman_collection.json
  format: json
  label: Nexxen DSP Location API
  slug: nexxen-dsp-location-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/tremor-video/refs/heads/main/collections/tremor-video.postman_collection.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Tremor Video Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Tremor Video secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Tremor Video
provider_slug: tremor-video
scheme_count: 1
schemes:
- applied_as: 'Authorization: Bearer <access_token>'
  applies_to:
  - https://services.amobee.com/campaign/v5/api
  - https://services.amobee.com/reporting/v2/api
  - https://services.amobee.com/device/v1/api
  - https://services.amobee.com/location/v1/api
  credentials:
  - client_id
  - client_secret
  flow: clientCredentials
  grant_type: client_credentials
  name: OAuth2ClientCredentials
  request_auth: none — the Token Service is the only DSP service that takes no access token
  request_body: JSON body {client_id, client_secret, grant_type=client_credentials}
  scopes: []
  sources:
  - collections/tremor-video.postman_collection.json
  - https://www.postman.com/nexxen-api/nexxen/documentation/9md8q3a/nexxen-dsp-apis
  tokenUrl: https://services.amobee.com/accounts/v1/api/token
  token_type: Bearer
  type: oauth2
slug: tremor-video-authentication
source_filename: tremor-video-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: collections/tremor-video.postman_collection.json\ndocs: https://www.postman.com/nexxen-api/nexxen/documentation/9md8q3a/nexxen-dsp-apis\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  token_type: Bearer\n  scopes_published: false\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  grant_type: client_credentials\n  tokenUrl: https://services.amobee.com/accounts/v1/api/token\n  credentials: [client_id, client_secret]\n  request_body: JSON body {client_id, client_secret, grant_type=client_credentials}\n  request_auth: none — the Token Service is the only DSP service that takes no access token\n  token_type: Bearer\n  applied_as: 'Authorization: Bearer <access_token>'\n  applies_to:\n  - https://services.amobee.com/campaign/v5/api\n  - https://services.amobee.com/reporting/v2/api\n  - https://services.amobee.com/device/v1/api\n  - https://services.amobee.com/location/v1/api\n\
  \  scopes: []\n  sources:\n  - collections/tremor-video.postman_collection.json\n  - https://www.postman.com/nexxen-api/nexxen/documentation/9md8q3a/nexxen-dsp-apis\ncredential_provisioning:\n  method: platform-provisioned\n  note: >-\n    client_id is the ID of an API service account and client_secret its password; both are created\n    inside the Nexxen / Amobee DSP platform by an existing customer. There is no self-serve\n    developer signup and no public key-issuance flow.\n  portal: https://login.amobee.com/portal/amobee/dsp/login\nfailure_mode:\n  status: 401\n  body: >-\n    {\"data\":[],\"errors\":[{\"message\":\"The \\\"Authorization\\\" header of the HTTP request is missing, or\n    specifies an expired or invalid access token.\",\"errorCode\":1,\"statusCode\":\"UNAUTHORIZED\"}]}\n  observed: live probe of https://services.amobee.com/campaign/v5/api/advertisers on 2026-08-13\ntoken_renewal:\n  method: re-POST the same request to the token endpoint\n  note: >-\n    An expired\
  \ token is replaced by re-sending the identical token request; the credentials do not\n    rotate. No refresh_token is issued (client-credentials).\nidentity_provider:\n  vendor: Okta\n  issuer: https://amobee-platform.okta.com/oauth2/default\n  discovery:\n  - well-known/tremor-video-openid-configuration.json\n  - well-known/tremor-video-oauth-authorization-server.json\n  token_format: JWT (RS256)\n  jwks_uri: https://amobee-platform.okta.com/oauth2/default/v1/keys\n  entitlement_claim: authorities\n  evidence: >-\n    The iss claim of the example access token Nexxen published in its own Postman collection, plus\n    the Content-Security-Policy on services.amobee.com, which allowlists amobee-platform.okta.com.\n  note: >-\n    Tokens are JWTs issued by Amobee/Nexxen's own Okta tenant and carry per-service entitlements in\n    an authorities[] claim rather than OAuth scopes. The Okta authorization server does not itself\n    advertise the client_credentials grant — services.amobee.com/accounts/v1/api/token\
  \ is the\n    supported wrapper and the only documented integration path.\n  ref: scopes/tremor-video-scopes.yml\ngateway:\n  name: Amobee Cloud Gateway\n  evidence: 'x-amobee-cloud-gateway: true and x-amobee-cloud-gateway-transaction-id on every response'\n  note: Authentication is enforced at the gateway, uniformly across all four DSP services.\nnotes: >-\n  The Nexxen DSP (formerly Amobee / Tremor Video DSP) API uses OAuth2 client-credentials with\n  Bearer tokens. There is no OpenID Connect discovery document, no OAuth authorization-server\n  metadata at /.well-known/oauth-authorization-server (404), and no published scope vocabulary — so\n  no scopes/ artifact is emitted. Authorization is per service account and per market rather than\n  per scope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tremor-video/refs/heads/main/authentication/tremor-video-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- MarTech
- Advertising
- AdTech
- DSP
- Programmatic
- CTV
- Video Advertising
---
