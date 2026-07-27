---
api_key_in:
- header
api_specs:
- filename: kore-wireless-connectivity-pro.yml
  format: yaml
  label: KORE Connectivity Pro API
  slug: kore-connectivity-pro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kore-wireless/refs/heads/main/openapi/kore-wireless-connectivity-pro.yml
- filename: kore-wireless-supersim.yml
  format: yaml
  label: KORE Super SIM API
  slug: kore-super-sim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kore-wireless/refs/heads/main/openapi/kore-wireless-supersim.yml
- filename: kore-wireless-programmable-wireless.yml
  format: yaml
  label: KORE Programmable Wireless API
  slug: kore-programmable-wireless-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kore-wireless/refs/heads/main/openapi/kore-wireless-programmable-wireless.yml
- filename: kore-wireless-sms.yml
  format: yaml
  label: KORE SMS API
  slug: kore-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kore-wireless/refs/heads/main/openapi/kore-wireless-sms.yml
- filename: kore-wireless-webhook.yml
  format: yaml
  label: KORE Webhook API
  slug: kore-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kore-wireless/refs/heads/main/openapi/kore-wireless-webhook.yml
- filename: kore-wireless-iam.yml
  format: yaml
  label: KORE Identity and Access Management API
  slug: kore-iam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kore-wireless/refs/heads/main/openapi/kore-wireless-iam.yml
- filename: kore-wireless-api-clients.yml
  format: yaml
  label: KORE API Clients API
  slug: kore-api-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kore-wireless/refs/heads/main/openapi/kore-wireless-api-clients.yml
- filename: kore-wireless-token.yml
  format: yaml
  label: KORE Token API
  slug: kore-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kore-wireless/refs/heads/main/openapi/kore-wireless-token.yml
auth_types:
- oauth2
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Kore Wireless Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: KORE Wireless secures its APIs with oauth2, apiKey, and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: KORE Wireless
provider_slug: kore-wireless
scheme_count: 3
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.korewireless.com/api-services/v1/auth/token
  name: Auth
  sources:
  - openapi/kore-wireless-api-clients.yml
  - openapi/kore-wireless-connectivity-pro.yml
  - openapi/kore-wireless-iam.yml
  - openapi/kore-wireless-programmable-wireless.yml
  - openapi/kore-wireless-sms.yml
  - openapi/kore-wireless-supersim.yml
  - openapi/kore-wireless-webhook.yml
  status: current
  type: oauth2
- in: header
  name: api_key
  note: Both specs declare an x-api-key header scheme alongside the OAuth scheme. The developer documentation describes only the OAuth 2.0 path, so treat the API key as a legacy developer-portal artifact rather than a supported alternative.
  parameter: x-api-key
  sources:
  - openapi/kore-wireless-connectivity-pro.yml
  - openapi/kore-wireless-sms.yml
  status: declared in spec, not documented
  type: apiKey
- name: accountSid_authToken
  note: The Super SIM spec retains the Twilio-era Account SID + Auth Token HTTP Basic scheme next to the KORE OAuth scheme. Migration guidance moves callers to KORE client credentials.
  scheme: basic
  sources:
  - openapi/kore-wireless-supersim.yml
  status: legacy (Twilio IoT inheritance)
  type: http
slug: kore-wireless-authentication
source_filename: kore-wireless-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: openapi/kore-wireless-api-clients.yml, openapi/kore-wireless-connectivity-pro.yml,\n  openapi/kore-wireless-iam.yml, openapi/kore-wireless-programmable-wireless.yml,\n  openapi/kore-wireless-sms.yml, openapi/kore-wireless-supersim.yml, openapi/kore-wireless-webhook.yml\ndocs: https://docs.korewireless.com/developers/api-management/auth\nclient_docs: https://docs.korewireless.com/developers/api-management/api-clients\nrefresh_guide: https://docs.korewireless.com/developers/how-to/apis/refresh-api-access-token\nsummary:\n  primary: oauth2 client_credentials\n  types: [oauth2, apiKey, http]\n  api_key_in: [header]\n  oauth2_flows: [clientCredentials]\n  bearer_header: 'Authorization: Bearer {access_token}'\n  credential_unit: API Client (Client ID + Client Secret), created per account in the\n    console\nprimary_flow:\n  name: OAuth 2.0 Client Credentials (RFC 6749 section 4.4)\n  token_endpoint: https://api.korewireless.com/api-services/v1/auth/token\n\
  \  method: POST\n  content_type: application/x-www-form-urlencoded\n  parameters: [grant_type=client_credentials, client_id, client_secret]\n  example_request: |\n    curl -X POST https://api.korewireless.com/api-services/v1/auth/token \\\n      --header 'cache-control: no-cache' \\\n      --header 'content-type: application/x-www-form-urlencoded' \\\n      --data \"grant_type=client_credentials\" \\\n      --data \"client_id=$KORE_CLIENT_ID\" \\\n      --data \"client_secret=$KORE_CLIENT_SECRET\"\n  response_shape: '{access_token, expires_in, token_type: Bearer, scope}'\n  token_format: RS256-signed JWT (iss/aud/sub/exp/iat/jti plus KORE claims account-id,\n    client-type, client_id, scopes)\n  expires_in_unit: seconds\n  expiry_options: [1 hour, 24 hours, 30 days, 24 months]\n  refresh: no refresh token — repeat the client-credentials exchange\n  spec: openapi/kore-wireless-token.yml\ncredentials:\n  where: API Client details in the KORE console (https://build.korewireless.com/clients/list)\n\
  \  client_secret_visibility: shown once at creation and never retrievable again\n  client_id_visibility: always visible\n  scoping: Client Type (Admin or Standard) plus selected Global Resources and Products\n  locking: a client can be locked so only Account Owner, Account Admins and the Client\n    Owner may edit it\n  per_account: a client targets exactly one account; child accounts each need their\n    own client\nerrors:\n- {stage: token exchange, http: 401, body: '{\"error\":\"unauthorized_client\",\"error_description\":\"Invalid\n    client or Invalid client credentials\"}'}\n- {stage: API call, http: 403, body: '{\"message\":\"User is not authorized to access\n    this resource with an explicit deny\",\"error\":\"Invalid or expired token\"}'}\nschemes:\n- name: Auth\n  type: oauth2\n  flows:\n  - {flow: clientCredentials, tokenUrl: 'https://api.korewireless.com/api-services/v1/auth/token',\n    scopes: 0}\n  sources:\n  - openapi/kore-wireless-api-clients.yml\n  - openapi/kore-wireless-connectivity-pro.yml\n\
  \  - openapi/kore-wireless-iam.yml\n  - openapi/kore-wireless-programmable-wireless.yml\n  - openapi/kore-wireless-sms.yml\n  - openapi/kore-wireless-supersim.yml\n  - openapi/kore-wireless-webhook.yml\n  status: current\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources: [openapi/kore-wireless-connectivity-pro.yml, openapi/kore-wireless-sms.yml]\n  status: declared in spec, not documented\n  note: >-\n    Both specs declare an x-api-key header scheme alongside the OAuth scheme. The\n    developer documentation describes only the OAuth 2.0 path, so treat the API key\n    as a legacy developer-portal artifact rather than a supported alternative.\n- name: accountSid_authToken\n  type: http\n  scheme: basic\n  sources: [openapi/kore-wireless-supersim.yml]\n  status: legacy (Twilio IoT inheritance)\n  note: >-\n    The Super SIM spec retains the Twilio-era Account SID + Auth Token HTTP Basic\n    scheme next to the KORE OAuth scheme. Migration guidance moves\
  \ callers to\n    KORE client credentials.\nwebhook_direction:\n  description: authenticity of KORE-to-customer callbacks is a separate contract —\n    KORE signs every event with the kore-signature header.\n  docs: https://docs.korewireless.com/developers/how-to/webhooks/validate-webhook-signatures\n  artifact: asyncapi/kore-wireless-event-streams-webhooks.yml\ncross_links:\n  scopes: scopes/kore-wireless-scopes.yml\n  conventions: conventions/kore-wireless-conventions.yml\n  errors: errors/kore-wireless-error-codes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kore-wireless/refs/heads/main/authentication/kore-wireless-authentication.yml
summary_line: oauth2/apiKey/http · 3 schemes
tags:
- Telecommunications
- United States
- IoT
- eSIM
- Connectivity
- MVNO
- SIM Management
- Roaming
- Messaging
- SMS
- Device Management
- Network APIs
---
