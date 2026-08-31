---
api_key_in:
- header
api_specs:
- filename: tata-communications-cdr-by-customer-message-id-api-openapi.yml
  format: yaml
  label: Tata Communications CDR by Customer Message Id API
  slug: tata-communications-cdr-by-customer-message-id-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tata-communications/refs/heads/main/openapi/tata-communications-cdr-by-customer-message-id-api-openapi.yml
- filename: tata-communications-destination-api-openapi.yml
  format: yaml
  label: Tata Communications Destination API
  slug: tata-communications-destination-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tata-communications/refs/heads/main/openapi/tata-communications-destination-api-openapi.yml
- filename: tata-communications-number-intelligence-api-openapi.yml
  format: yaml
  label: Tata Communications Number Intelligence API
  slug: tata-communications-number-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tata-communications/refs/heads/main/openapi/tata-communications-number-intelligence-api-openapi.yml
- filename: tata-communications-report-api-openapi.yml
  format: yaml
  label: Tata Communications Report API
  slug: tata-communications-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tata-communications/refs/heads/main/openapi/tata-communications-report-api-openapi.yml
- filename: tata-communications-senderid-api-openapi.yml
  format: yaml
  label: Tata Communications Sender ID API
  slug: tata-communications-senderid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tata-communications/refs/heads/main/openapi/tata-communications-senderid-api-openapi.yml
- filename: tata-communications-top-25-cdr-by-account-id-time-frame-api-openapi.yml
  format: yaml
  label: Tata Communications TOP 25 CDR by account Id & Time Frame API
  slug: tata-communications-top-25-cdr-by-account-id-time-frame-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tata-communications/refs/heads/main/openapi/tata-communications-top-25-cdr-by-account-id-time-frame-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Tata Communications Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Tata Communications secures its APIs with apiKey and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Tata Communications
provider_slug: tata-communications
scheme_count: 4
schemes:
- evidence: The Number Intelligence API declares a required header parameter named "Authorization" with the description "used for authentication in Akana". It is an operation parameter, not a securityDefinitions entry, so no scheme type, no token format, and no token endpoint are machine-readable.
  in: header
  name: Akana Authorization header
  parameter: Authorization
  required: true
  sources:
  - openapi/tata-communications-number-intelligence-api.json
  spec_declared: false
  type: apiKey
  where: developer.tatacommunications.com (Akana Community Manager)
- evidence: All three Mobile Messaging Exchange Account Administration operations carry an "appid" header parameter, which is the Akana Community Manager application identifier issued when an app is registered against an API contract.
  in: header
  name: Akana application id header
  parameter: appid
  required: false
  sources:
  - openapi/tata-communications-mobile-messaging-exchange-account-administration.json
  spec_declared: false
  type: apiKey
  where: developer.tatacommunications.com (Akana Community Manager)
- evidence: The MOVE developer portal publishes a dedicated "Move Access Token API — API to generate Access Token (OAuth 2.0 bearer token) to access Move APIs" alongside the MOVE SIM Connect and MOVE IOT Connect APIs. The token API's own reference is behind portal sign-in, so the grant type, token endpoint URL, and any scope list are not anonymously verifiable; no RFC 8414 or OpenID Connect discovery document is served on the host.
  flow: clientCredentials
  name: MOVE OAuth 2.0 bearer token
  scopes_published: false
  spec_declared: false
  token_api: https://move-external-apim-prod.developer.azure-api.net/api-details#api=tata-move-api-access-manager
  type: oauth2
  where: MOVE (Azure API Management, move-external-apim-prod)
- evidence: '"You will need auth token to access our APIs. Please fill in your details below and we will get in touch with you." Access to the DIGO CPaaS APIs is sales-led; there is no self-serve credential issuance and no published token endpoint.'
  in: header
  name: DIGO auth token (issued on request)
  self_serve: false
  spec_declared: false
  type: apiKey
  where: DIGO CPaaS (tatacommunicationsdigo.io)
slug: tata-communications-authentication
source_filename: tata-communications-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: >-\n  openapi/*.json (Swagger 2.0 harvested from developer.tatacommunications.com),\n  https://www.developer.move.tatacommunications.com/,\n  https://tatacommunicationsdigo.io/documentation-api/\ndocs: https://developer.tatacommunications.com/\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  spec_declared_security_schemes: 0\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\n  note: >-\n    None of the three anonymously downloadable Swagger 2.0 documents declares a\n    securityDefinitions block, so this profile is searched from the operation parameters\n    and the provider's own product documentation rather than derived mechanically. Tata\n    Communications runs three separate authentication regimes across three separate\n    developer properties; there is no single account, no single token, and no shared\n    identity provider between them.\nschemes:\n- name: Akana Authorization header\n  type: apiKey\n \
  \ in: header\n  parameter: Authorization\n  where: developer.tatacommunications.com (Akana Community Manager)\n  required: true\n  spec_declared: false\n  sources:\n  - openapi/tata-communications-number-intelligence-api.json\n  evidence: >-\n    The Number Intelligence API declares a required header parameter named \"Authorization\"\n    with the description \"used for authentication in Akana\". It is an operation parameter,\n    not a securityDefinitions entry, so no scheme type, no token format, and no token\n    endpoint are machine-readable.\n- name: Akana application id header\n  type: apiKey\n  in: header\n  parameter: appid\n  where: developer.tatacommunications.com (Akana Community Manager)\n  required: false\n  spec_declared: false\n  sources:\n  - openapi/tata-communications-mobile-messaging-exchange-account-administration.json\n  evidence: >-\n    All three Mobile Messaging Exchange Account Administration operations carry an \"appid\"\n    header parameter, which is the Akana\
  \ Community Manager application identifier issued\n    when an app is registered against an API contract.\n- name: MOVE OAuth 2.0 bearer token\n  type: oauth2\n  flow: clientCredentials\n  where: MOVE (Azure API Management, move-external-apim-prod)\n  spec_declared: false\n  token_api: https://move-external-apim-prod.developer.azure-api.net/api-details#api=tata-move-api-access-manager\n  scopes_published: false\n  evidence: >-\n    The MOVE developer portal publishes a dedicated \"Move Access Token API — API to generate\n    Access Token (OAuth 2.0 bearer token) to access Move APIs\" alongside the MOVE SIM Connect\n    and MOVE IOT Connect APIs. The token API's own reference is behind portal sign-in, so the\n    grant type, token endpoint URL, and any scope list are not anonymously verifiable; no\n    RFC 8414 or OpenID Connect discovery document is served on the host.\n- name: DIGO auth token (issued on request)\n  type: apiKey\n  in: header\n  where: DIGO CPaaS (tatacommunicationsdigo.io)\n\
  \  spec_declared: false\n  self_serve: false\n  evidence: >-\n    \"You will need auth token to access our APIs. Please fill in your details below and we\n    will get in touch with you.\" Access to the DIGO CPaaS APIs is sales-led; there is no\n    self-serve credential issuance and no published token endpoint.\ngaps:\n- No securityDefinitions/securitySchemes in any published specification.\n- No OAuth scope reference is published for MOVE, so no scopes/ artifact is emitted.\n- No mutual TLS, no OpenID Connect, and no CIBA surface is documented anywhere.\n- No anonymous sign-up path on the first-party Akana portal; the MOVE portal exposes\n  /signin and /signup but everything behind them is gated.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tata-communications/refs/heads/main/authentication/tata-communications-authentication.yml
summary_line: apiKey/oauth2 · 4 schemes
tags:
- Telecommunications
- India
- Wholesale Carrier
- CPaaS
- Messaging
- Voice
- IoT
- eSIM
- Number Intelligence
- Connectivity
- Subsea Cable
- Partner Gated
---
