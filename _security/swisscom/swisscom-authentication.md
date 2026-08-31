---
api_key_in: []
api_specs:
- filename: swisscom-process-create-api-openapi.yml
  format: yaml
  label: 'Swisscom Process: create API'
  slug: swisscom-process-create-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swisscom/refs/heads/main/openapi/swisscom-process-create-api-openapi.yml
- filename: swisscom-process-read-api-openapi.yml
  format: yaml
  label: 'Swisscom Process: read API'
  slug: swisscom-process-read-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swisscom/refs/heads/main/openapi/swisscom-process-read-api-openapi.yml
- filename: swisscom-signatures-api-openapi.yml
  format: yaml
  label: Swisscom Signatures API
  slug: swisscom-signatures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swisscom/refs/heads/main/openapi/swisscom-signatures-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Swisscom Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Swisscom secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Swisscom
provider_slug: swisscom
scheme_count: 1
schemes:
- description: OAuth 2.0 Client Credentials flow for accessing the Swisscom Sign Integration API.
  flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://sign.swisscom.ch/realms/swisscom-public/protocol/openid-connect/token
  name: SwisscomSignOAuth2
  sources:
  - openapi/swisscom-sign-integration-api-openapi.json
  type: oauth2
slug: swisscom-authentication
source_filename: swisscom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: openapi/swisscom-sign-integration-api-openapi.json\ndocs: https://sign.swisscom.ch/docs/guide/authentication\nportal_docs: https://digital.swisscom.com/resources/use-your-api-keys/oaut-introduction\nlegacy_docs: https://github.com/swisscom-api/doc/wiki/oauth-overview.html\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: SwisscomSignOAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://sign.swisscom.ch/realms/swisscom-public/protocol/openid-connect/token\n    scopes: 3\n  description: OAuth 2.0 Client Credentials flow for accessing the Swisscom Sign Integration\n    API.\n  sources:\n  - openapi/swisscom-sign-integration-api-openapi.json\noidc:\n  discovery: https://sign.swisscom.ch/realms/swisscom-public/.well-known/openid-configuration\n  harvested: well-known/swisscom-sign-openid-configuration.json\n  issuer: https://sign.swisscom.ch/realms/swisscom-public\n\
  \  jwks_uri: https://sign.swisscom.ch/realms/swisscom-public/protocol/openid-connect/certs\n  provider: Keycloak (realm swisscom-public)\n  audience: swisscom-sign-api\n  tenancy_claim: organization_id\nexample_token_request: |\n  curl --request POST \\\n    --url https://sign.swisscom.ch/realms/swisscom-public/protocol/openid-connect/token \\\n    --header 'content-type: application/x-www-form-urlencoded' \\\n    --data 'grant_type=client_credentials&client_id=YOUR_CLIENT_ID&client_secret=YOUR_CLIENT_SECRET'\nguidance: >-\n  Swisscom recommends calling Swisscom Sign from your own backend so client credentials stay\n  server-side. Its browser-based API explorer accepts client_id and client_secret client-side and is\n  documented as a controlled-testing tool only, not a production integration pattern.\nother_surfaces:\n- surface: swisscom-all-in-signing-service\n  spec: openapi/swisscom-all-in-signing-service-openapi.yml\n  types: [mutualTLS]\n  detail: >-\n    The published OpenAPI declares\
  \ no securitySchemes. Access is authenticated with a client\n    certificate issued under a Swisscom Trust Services contract; the request body carries a SAD\n    (signature activation data) token authorising the signer, plus a provisioned credentialID.\n  spec_gap: true\n- surface: api.swisscom.com-marketplace-gateway\n  spec: null\n  types: [apiKey, oauth2]\n  detail: >-\n    A client_id header authenticates the messaging products (Text Messaging, Token Validation,\n    added-value SMS short-ID lookups). OAuth 2.0 client credentials authenticate the Mobility\n    Insights products (Heatmaps, Dwell Times, Origin Destination). The legacy Voice APIs use\n    authorization-code or implicit grants via https://consent.swisscom.com. The Swiss AI Platform\n    inference endpoints are API-key authenticated and require a signed service contract.\n  authorization_endpoint: https://consent.swisscom.com/c/oauth2/auth\n  token_endpoint: https://consent.swisscom.com/o/oauth2/token\n  docs: https://digital.swisscom.com/resources/use-your-api-keys/oaut-introduction\n\
  scopes_detail: scopes/swisscom-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swisscom/refs/heads/main/authentication/swisscom-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Telecommunications
- Switzerland
- Mobile Network Operator
- Broadband
- Network APIs
- Open Gateway
- Messaging
- SMS
- Voice
- Identity Verification
- Mobility Data
- Digital Signatures
- eSIM
- Artificial Intelligence
---
