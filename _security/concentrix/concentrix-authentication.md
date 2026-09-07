---
anonymous_access: false
api_key_in:
- header
auth_types:
- http
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Concentrix Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: Concentrix secures its APIs with http and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: Concentrix
provider_slug: concentrix
scheme_count: 2
schemes:
- applies_to:
  - iX Hello Customer v2 Universal Messaging API (headless flow execution)
  - iX Hello Customer v2 Outbound Calling API
  description: '"Authorization: Bearer <api_key>". API keys are provisioned per organization, stored in the platform''s Secrets Manager, and shared between the Headless Flow Execution API and the Outbound Calling API. The platform validates the orgId in every request path against the key; a key cannot reach flows or call records belonging to another organization.'
  errors:
  - code: AUTH_HEADER_MISSING
    meaning: Authorization header was not provided
    status: 401
  - code: INVALID_TOKEN
    meaning: API key is invalid
    or expired: null
    revoked: null
    status: 401
  - code: PERMISSION_DENIED
    meaning: org lacks the outbound_calling permission
    or the flow belongs to a different org: null
    status: 403
  in: header
  name: ixHelloApiKey
  parameter: Authorization
  provisioning: contact the iX Hello product team — no self-service key issuance is documented
  scheme: bearer
  sources:
  - https://docs.ixhello.com/ixhc2/integrations/outbound-calling-api-user-guide
  - https://docs.ixhello.com/ixhc2/integrations/executing-flow-via-api-headless-execution
  type: http
- authorization_endpoint: https://ixadminprodk5.b2clogin.com/2c95ae7b-5bab-49e0-a483-62a3cd3867ba/b2c_1a_signup_signin/oauth2/v2.0/authorize
  claims_supported:
  - sub
  - tid
  - name
  - email
  - orgId
  - orgName
  - zoneinfo
  - locale
  - citizenOf
  - given_name
  - family_name
  - iss
  - iat
  - exp
  - aud
  - acr
  - nonce
  - auth_time
  description: Azure AD B2C tenant fronting interactive sign-in to the iX Hello application (www.ixhello.com). Discovery document fetched anonymously and saved verbatim to well-known/concentrix-openid-configuration.json.
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://ixadminprodk5.b2clogin.com/tfp/2c95ae7b-5bab-49e0-a483-62a3cd3867ba/b2c_1a_signup_signin/v2.0/
  jwks_uri: https://ixadminprodk5.b2clogin.com/2c95ae7b-5bab-49e0-a483-62a3cd3867ba/b2c_1a_signup_signin/discovery/v2.0/keys
  name: ixPlatformB2C
  openIdConnectUrl: https://ixadminprodk5.b2clogin.com/2c95ae7b-5bab-49e0-a483-62a3cd3867ba/b2c_1a_signup_signin/v2.0/.well-known/openid-configuration
  scopes_supported:
  - openid
  sources:
  - well-known/concentrix-openid-configuration.json
  token_endpoint: https://ixadminprodk5.b2clogin.com/2c95ae7b-5bab-49e0-a483-62a3cd3867ba/b2c_1a_signup_signin/oauth2/v2.0/token
  type: openIdConnect
slug: concentrix-authentication
source_filename: concentrix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: https://docs.ixhello.com/ixhc2/integrations/outbound-calling-api-user-guide\ndocs: https://docs.ixhello.com/ixhc2/integrations/outbound-calling-api-user-guide\nnote: >-\n  Concentrix publishes no OpenAPI, so this profile is read from the iX Hello Customer v2\n  documentation rather than derived from securitySchemes. Two distinct auth surfaces exist:\n  (1) organization-scoped API keys presented as a bearer token on the public iX Hello Customer v2\n  APIs, and (2) Azure AD B2C OpenID Connect for interactive sign-in to the iX Hello application.\nsummary:\n  types: [http, openIdConnect]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, implicit]\nschemes:\n  - name: ixHelloApiKey\n    type: http\n    scheme: bearer\n    in: header\n    parameter: Authorization\n    description: >-\n      \"Authorization: Bearer <api_key>\". API keys are provisioned per organization, stored in the\n      platform's Secrets Manager, and\
  \ shared between the Headless Flow Execution API and the\n      Outbound Calling API. The platform validates the orgId in every request path against the key;\n      a key cannot reach flows or call records belonging to another organization.\n    applies_to:\n      - iX Hello Customer v2 Universal Messaging API (headless flow execution)\n      - iX Hello Customer v2 Outbound Calling API\n    provisioning: contact the iX Hello product team — no self-service key issuance is documented\n    sources:\n      - https://docs.ixhello.com/ixhc2/integrations/outbound-calling-api-user-guide\n      - https://docs.ixhello.com/ixhc2/integrations/executing-flow-via-api-headless-execution\n    errors:\n      - {status: 401, code: AUTH_HEADER_MISSING, meaning: Authorization header was not provided}\n      - {status: 401, code: INVALID_TOKEN, meaning: API key is invalid, revoked, or expired}\n      - {status: 403, code: PERMISSION_DENIED, meaning: org lacks the outbound_calling permission, or the flow belongs\
  \ to a different org}\n  - name: ixPlatformB2C\n    type: openIdConnect\n    openIdConnectUrl: https://ixadminprodk5.b2clogin.com/2c95ae7b-5bab-49e0-a483-62a3cd3867ba/b2c_1a_signup_signin/v2.0/.well-known/openid-configuration\n    description: >-\n      Azure AD B2C tenant fronting interactive sign-in to the iX Hello application\n      (www.ixhello.com). Discovery document fetched anonymously and saved verbatim to\n      well-known/concentrix-openid-configuration.json.\n    issuer: https://ixadminprodk5.b2clogin.com/tfp/2c95ae7b-5bab-49e0-a483-62a3cd3867ba/b2c_1a_signup_signin/v2.0/\n    authorization_endpoint: https://ixadminprodk5.b2clogin.com/2c95ae7b-5bab-49e0-a483-62a3cd3867ba/b2c_1a_signup_signin/oauth2/v2.0/authorize\n    token_endpoint: https://ixadminprodk5.b2clogin.com/2c95ae7b-5bab-49e0-a483-62a3cd3867ba/b2c_1a_signup_signin/oauth2/v2.0/token\n    jwks_uri: https://ixadminprodk5.b2clogin.com/2c95ae7b-5bab-49e0-a483-62a3cd3867ba/b2c_1a_signup_signin/discovery/v2.0/keys\n    scopes_supported:\
  \ [openid]\n    id_token_signing_alg_values_supported: [RS256]\n    claims_supported: [sub, tid, name, email, orgId, orgName, zoneinfo, locale, citizenOf, given_name, family_name, iss, iat, exp, aud, acr, nonce, auth_time]\n    sources:\n      - well-known/concentrix-openid-configuration.json\nwebhook_authentication:\n  mechanism: HMAC-SHA256 payload signature\n  header: X-Signature\n  format: sha256=<hex>\n  secret: caller-supplied \"webhookAuth\" value from the call-initiation request\n  computation: HMAC-SHA256(webhookAuth, rawRequestBody)\n  note: >-\n    webhookAuth is NOT forwarded as an Authorization header — it only signs the payload. If it is\n    omitted the callback is still sent, signed with an empty secret (effectively unsigned).\n  source: https://docs.ixhello.com/ixhc2/integrations/outbound-calling-api-user-guide\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/concentrix/refs/heads/main/authentication/concentrix-authentication.yml
summary_line: http/openIdConnect · 2 schemes
tags:
- AI Agents
- Business Process Outsourcing
- Consulting
- Conversational AI
- Customer Experience
- Digital Transformation
- Enterprise Services
- Contact Center
- Voice
- Webhooks
- Fortune 500
---
