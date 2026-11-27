---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nexpay-com-au-openapi-generated.yml
  format: yaml
  label: NexPay API
  slug: nexpay-com-au-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexpay-com-au/openapi/_ae-authored/nexpay-com-au-openapi-generated.yml
auth_types: []
description: Authentication schemes for NexPay APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: NexPay Authentication
name_suffix: Authentication
oauth_flows: []
overview: NexPay declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: NexPay
provider_slug: nexpay-com-au
scheme_count: 2
schemes:
- evidence: 'Nexpay authenticates server-to-server (M2M) traffic using API keys . Each key is a pair: a public clientId and a private secret . The two are combined and sent on the X-API-Key header of every request.'
  header: X-API-Key
  how_to_obtain: Create an API key via the dashboard or POST /v2/dev/api-keys endpoint; the response returns a clientId and secret.
  location: header
  name: X-API-Key
  type: other
- evidence: 'Authorization: Bearer <token> — for browser sessions, where a human user has logged into the Nexpay Dashboard. Tokens are issued by POST /v2/auth/login and short-lived.'
  flows:
  - client_credentials
  header: Authorization
  how_to_obtain: Obtain a token by calling POST /v2/auth/login with user credentials.
  location: header
  name: Bearer token
  type: http-bearer
slug: nexpay-com-au-authentication
source_filename: nexpay-com-au-authentication.yml
source_heading: Authentication Profile
source_url: https://nexpay.com.au/training/team-and-account/api-keys-and-integrations/
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://nexpay.com.au/training/team-and-account/api-keys-and-integrations/\nsources:\n- https://nexpay.com.au/training/team-and-account/api-keys-and-integrations/\n- https://nexpay.com.au/training/team-and-account/api-keys-and-integrations.md\n- https://docs.nexpay.com.au/docs/api-keys\n- https://docs.nexpay.com.au/docs/authentication\ndescription: Authentication schemes for NexPay APIs\nschemes:\n- type: other\n  name: X-API-Key\n  evidence: 'Nexpay authenticates server-to-server (M2M) traffic using API keys . Each key is a pair: a public clientId and a private secret .\n    The two are combined and sent on the X-API-Key header of every request.'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create an API key via the dashboard or POST /v2/dev/api-keys endpoint; the response returns a clientId and secret.\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Authorization:\
  \ Bearer <token> — for browser sessions, where a human user has logged into the Nexpay Dashboard. Tokens are issued\n    by POST /v2/auth/login and short-lived.'\n  location: header\n  header: Authorization\n  flows:\n  - client_credentials\n  how_to_obtain: Obtain a token by calling POST /v2/auth/login with user credentials.\ndocs: https://nexpay.com.au/training/team-and-account/api-keys-and-integrations/\n"
source_yaml_url: https://artifacts.apis.io/nexpay-com-au/authentication/nexpay-com-au-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Payments
- Education
- International
- Fintech
---
