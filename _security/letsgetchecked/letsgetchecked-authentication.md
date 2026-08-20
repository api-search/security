---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Letsgetchecked Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: LetsGetChecked secures its APIs with oauth2 and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: LetsGetChecked
provider_slug: letsgetchecked
scheme_count: 3
schemes:
- credential_format: alphanumeric, 25 characters each
  credential_model: access key ID + secret access key
  credential_transport: HTTP Basic (curl --user <access key>:<secret key>)
  flow: clientCredentials
  grant_type: client_credentials
  name: OAuth2ClientCredentials
  request_content_type: application/x-www-form-urlencoded
  scopes: []
  scopes_note: No scopes are used. The 14 September 2023 release notes record "Remove scope from example to request an access token", so the scope parameter was explicitly withdrawn from the flow. There is no permissions or scopes reference page, which is why this repo carries no scopes/ artifact.
  sources:
  - https://docs.letsgetchecked.com/documentation/API%20Reference/Getting%20Started/authentication-flow/
  token_endpoint: '{LGC-API}/oauth2/token'
  token_endpoint_note: The host is templated as {LGC-API} throughout the documentation. LetsGetChecked does not publish the production or staging API hostname; it is supplied privately per client during onboarding.
  type: oauth2
- bearer_format: JWT
  description: The access token returned by the token endpoint is presented as a bearer token on every API operation. The documented sample sends the raw token value in the Authorization header. Expired or invalid tokens return HTTP 401.
  in: header
  name: BearerToken
  parameter_name: Authorization
  scheme: bearer
  sources:
  - https://docs.letsgetchecked.com/documentation/API%20Reference/Getting%20Started/authentication-flow/
  token_lifetime: Returned alongside the token as a validity value; no fixed TTL is published.
  type: http
- algorithm: HMAC-SHA256
  direction: inbound-to-client
  encoding: base64
  in: header
  key_supply: The client generates a strong signing key in base64 and supplies it to LetsGetChecked during onboarding.
  name: WebhookHMACSignature
  optional: true
  optional_note: Signing is opt-in. The documentation states that authentication mechanisms are not required for submitted payloads "due to their lightweight content", and instructs clients to inspect the callback URL to avoid leaking access tokens. Signature verification is only applied when the client requests it.
  parameter_name: Authorization
  reference: https://www.rfc-editor.org/rfc/rfc2104
  scheme: LGC2-HMAC-SHA256
  signed_content: the stringified JSON request body
  sources:
  - https://docs.letsgetchecked.com/documentation/API%20Reference/API%20Notifications/security/
  type: http
slug: letsgetchecked-authentication
source_filename: letsgetchecked-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://docs.letsgetchecked.com/documentation/API%20Reference/Getting%20Started/authentication-flow/\ndocs: https://docs.letsgetchecked.com/documentation/API%20Reference/Getting%20Started/authentication-flow/\n\n# Derived from the published authentication documentation, not from an OpenAPI\n# securityScheme block — LetsGetChecked publishes no machine-readable specification.\n\nsummary:\n  types:\n  - oauth2\n  - http\n  oauth2_flows:\n  - clientCredentials\n  bearer_format: JWT\n  api_key_in: []\n  scopes_used: false\n  mutual_tls: false\n  openid_connect: false\n  credential_issuance: manual\n  self_service_signup: false\n\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_endpoint: '{LGC-API}/oauth2/token'\n  token_endpoint_note: 'The host is templated as {LGC-API} throughout the documentation.\n    LetsGetChecked does not publish the production or staging API hostname; it is\n\
  \    supplied privately per client during onboarding.'\n  grant_type: client_credentials\n  credential_model: access key ID + secret access key\n  credential_format: alphanumeric, 25 characters each\n  credential_transport: HTTP Basic (curl --user <access key>:<secret key>)\n  request_content_type: application/x-www-form-urlencoded\n  scopes: []\n  scopes_note: 'No scopes are used. The 14 September 2023 release notes record \"Remove\n    scope from example to request an access token\", so the scope parameter was\n    explicitly withdrawn from the flow. There is no permissions or scopes reference\n    page, which is why this repo carries no scopes/ artifact.'\n  sources:\n  - https://docs.letsgetchecked.com/documentation/API%20Reference/Getting%20Started/authentication-flow/\n\n- name: BearerToken\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  in: header\n  parameter_name: Authorization\n  description: 'The access token returned by the token endpoint is presented as a bearer\n\
  \    token on every API operation. The documented sample sends the raw token value in\n    the Authorization header. Expired or invalid tokens return HTTP 401.'\n  token_lifetime: 'Returned alongside the token as a validity value; no fixed TTL is\n    published.'\n  sources:\n  - https://docs.letsgetchecked.com/documentation/API%20Reference/Getting%20Started/authentication-flow/\n\n- name: WebhookHMACSignature\n  type: http\n  scheme: LGC2-HMAC-SHA256\n  direction: inbound-to-client\n  in: header\n  parameter_name: Authorization\n  algorithm: HMAC-SHA256\n  encoding: base64\n  signed_content: the stringified JSON request body\n  key_supply: 'The client generates a strong signing key in base64 and supplies it to\n    LetsGetChecked during onboarding.'\n  optional: true\n  optional_note: 'Signing is opt-in. The documentation states that authentication\n    mechanisms are not required for submitted payloads \"due to their lightweight\n    content\", and instructs clients to inspect the callback\
  \ URL to avoid leaking\n    access tokens. Signature verification is only applied when the client requests it.'\n  reference: https://www.rfc-editor.org/rfc/rfc2104\n  sources:\n  - https://docs.letsgetchecked.com/documentation/API%20Reference/API%20Notifications/security/\n\nenvironments:\n- name: staging\n  access: 'Credentials issued by LetsGetChecked. The staging server is IP-restricted;\n    LetsGetChecked shares the staging server IP address with the client.'\n- name: production\n  access: 'Production credentials are issued only after LetsGetChecked has verified the\n    client integration against staging.'\n\ngaps:\n- No self-service credential issuance or developer sign-up for the B2B API.\n- No published API hostname for either environment.\n- No OAuth scopes, so authorization is all-or-nothing per client credential.\n- No token revocation, rotation, or introspection endpoint documented.\n- No .well-known/oauth-authorization-server or openid-configuration on any\n  LetsGetChecked\
  \ host (see well-known/letsgetchecked-well-known.yml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/letsgetchecked/refs/heads/main/authentication/letsgetchecked-authentication.yml
summary_line: oauth2/http · 3 schemes
tags:
- Company
- Health
- Healthcare
- Diagnostics
- Laboratory
- Telehealth
- Medical Testing
- Pharmacy
- Order
- Results
- Webhook
- HL7
- LOINC
---
