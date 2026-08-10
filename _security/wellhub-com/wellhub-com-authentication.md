---
api_key_in: []
api_specs:
- filename: wellhub-com-integrations-openapi-original.json
  format: json
  label: Wellhub Integrations API
  slug: wellhub-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellhub-com/refs/heads/main/openapi/wellhub-com-integrations-openapi-original.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Wellhub Com Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Wellhub secures its APIs with http and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Wellhub
provider_slug: wellhub-com
scheme_count: 1
schemes:
- applied_to: every operation except POST /oauth/token
  bearerFormat: JWT
  description: Bearer token obtained from `POST /oauth/token` using the client_credentials grant type.
  name: OAuth2
  scheme: bearer
  sources:
  - openapi/wellhub-com-integrations-openapi-original.json
  type: http
slug: wellhub-com-authentication
source_filename: wellhub-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: openapi/wellhub-com-integrations-openapi-original.json\ndocs: https://developer-hub.wellhub.com/docs/integrations/api/getting-started\nsummary:\n  types:\n  - http\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - clientCredentials\n  note: >-\n    The contract models authentication as a plain `http`/`bearer` scheme, but the flow Wellhub\n    documents and implements is OAuth 2.0 client credentials — the bearer token is minted by\n    POST /oauth/token, which is itself declared as an operation in the same contract rather than as\n    an oauth2 securityScheme with a tokenUrl. Both facts are recorded below.\nschemes:\n- name: OAuth2\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token obtained from `POST /oauth/token` using the client_credentials grant type.\n  sources:\n  - openapi/wellhub-com-integrations-openapi-original.json\n  applied_to: every operation except POST /oauth/token\nflow:\n  grant_type:\
  \ client_credentials\n  token_endpoint: https://api.clients.wellhub.com/oauth/token\n  token_endpoint_sandbox: https://pilot-api.clients.wellhub.com/oauth/token\n  request_content_type: application/x-www-form-urlencoded\n  request_params:\n  - {name: client_id, required: true, description: Your OAuth client ID.}\n  - {name: client_secret, required: true, description: Your OAuth client secret.}\n  - {name: grant_type, required: true, value: client_credentials}\n  response_fields: [access_token, token_type, expires_in]\n  token_type: Bearer\n  token_lifetime_seconds: 3600\n  refresh_token: false\n  pkce: false\n  rate_limit: 5 requests per minute / 5 requests per second burst\n  usage_header: 'Authorization: Bearer <access_token>'\n  error_statuses: [400, 401, 403, 500]\ncredentials:\n  issuer: Wellhub for Companies portal\n  portal: https://clients.gympass.com/\n  path: Settings → API OAuth credentials → Generate credential\n  attributes:\n  - {name: Credential name, description: Free-text\
  \ label identifying the integration.}\n  - {name: Data access, values: [Production, Sandbox], description: 'Selects live data or the synthetic-data sandbox. Set at creation; not switchable per request.'}\n  - {name: Credential expiration, description: 'A fixed duration, or \"Never expire\".'}\n  - {name: Permissions, description: Access level chosen per product area at creation time.}\n  secret_shown_once: true\n  rotation: Self-service from the API OAuth credentials page in the portal.\n  handling_policy: >-\n    Wellhub states it will never ask for a Client Secret through any channel — email, chat, phone or\n    support ticket — and that any such request should be treated as phishing and reported.\nscopes:\n  published: false\n  model: per-product-area permissions selected on the credential\n  note: >-\n    Wellhub publishes no OAuth scope names. Authorization granularity is set when the credential is\n    created (product area + access level) rather than requested per token, so there\
  \ is no scope\n    parameter and no scopes/ artifact. See conformance/wellhub-com-conformance.yml (oauth2-scopes).\nnetwork_controls:\n  ip_validation: true\n  description: >-\n    Wellhub validates the calling integration's source IPs against its security guidelines. Requests\n    from addresses that fall under bot or anonymizer rules can be rejected with 403 Forbidden.\n  self_service: false\n  remediation: Contact your Wellhub team so the IP can be reviewed internally. There is no self-service allowlist.\ndiscovery:\n  oauth_authorization_server_metadata: false\n  openid_configuration: false\n  note: Neither RFC 8414 nor OIDC discovery is served on any host. See well-known/wellhub-com-well-known.yml.\nx-evidence:\n  fetched: '2026-08-04'\n  probes:\n  - {url: 'https://api.clients.wellhub.com/oauth/token', method: POST, body: 'grant_type=client_credentials', http_status: 401, response: '{\"error\":\"Unauthorized\"}'}\n  - {url: 'https://api.clients.wellhub.com/v1/companies', method:\
  \ GET, http_status: 401, response: '{\"error\":\"Jwt is missing\",\"path\":\"/v1/companies\",\"status_code\":401}'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wellhub-com/refs/heads/main/authentication/wellhub-com-authentication.yml
summary_line: http/oauth2 · 1 scheme
tags:
- Company
- corporate-wellness
- employee-benefits
- human-resources
- hr-tech
- eligibility
- workforce
- fitness
- wellbeing
- payroll
- sftp
- hris-integration
---
