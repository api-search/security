---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: difficat-com-balance-api-openapi.yml
  format: yaml
  label: DiffiCat Balance API
  slug: difficat-com-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/difficat-com/openapi/difficat-com-balance-api-openapi.yml
- filename: difficat-com-compares-api-openapi.yml
  format: yaml
  label: DiffiCat Compares API
  slug: difficat-com-compares-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/difficat-com/openapi/difficat-com-compares-api-openapi.yml
- filename: difficat-com-discover-api-openapi.yml
  format: yaml
  label: DiffiCat Discover API
  slug: difficat-com-discover-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/difficat-com/openapi/difficat-com-discover-api-openapi.yml
- filename: difficat-com-feedback-api-openapi.yml
  format: yaml
  label: DiffiCat Feedback API
  slug: difficat-com-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/difficat-com/openapi/difficat-com-feedback-api-openapi.yml
- filename: difficat-com-jobs-api-openapi.yml
  format: yaml
  label: DiffiCat Jobs API
  slug: difficat-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/difficat-com/openapi/difficat-com-jobs-api-openapi.yml
- filename: difficat-com-screenshots-api-openapi.yml
  format: yaml
  label: DiffiCat Screenshots API
  slug: difficat-com-screenshots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/difficat-com/openapi/difficat-com-screenshots-api-openapi.yml
- filename: difficat-com-snapshots-api-openapi.yml
  format: yaml
  label: DiffiCat Snapshots API
  slug: difficat-com-snapshots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/difficat-com/openapi/difficat-com-snapshots-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 6
method: searched
name: DiffiCat Authentication
name_suffix: Authentication
oauth_flows: []
overview: DiffiCat secures its APIs with apiKey and http across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DiffiCat
provider_slug: difficat-com
scheme_count: 6
schemes:
- description: 'Machine Payments Protocol (mpp.dev). A first request without a credential is answered with 402 and a WWW-Authenticate: Payment challenge; the paid retry carries Authorization: Payment <credential>. Successful responses carry a Payment-Receipt header. x402 clients are accepted on the same routes for USDC on Base. Over MCP the challenge is JSON-RPC error -32042 and the credential travels in _meta["org.paymentauth/credential"].'
  name: payment
  scheme: Payment
  sources:
  - openapi/difficat-com-openapi.yml
  - https://difficat.com/llms.txt
  type: http
- alternate_header: X-DiffiCat-Key
  description: 'A prepaid key (dck_…) from the account page at /account, where a signed-in human tops up by card through Stripe Checkout and copies the key. Sent as Authorization: Bearer dck_…; on MCP a gateway that cannot set Authorization may send it as X-DiffiCat-Key. An insufficient balance answers 402, an unknown key 401.'
  key_prefix: dck_
  name: prepaidKey
  scheme: bearer
  sources:
  - openapi/difficat-com-openapi.yml
  - https://difficat.com/llms.txt
  type: http
- description: A Pro account's API key draws on the 5,000 captured pages a month included in Pro, with overage billed up to a cap set on the account page.
  name: proKey
  scheme: bearer
  sources:
  - https://difficat.com/llms.txt
  type: http
- description: The one-time jobToken returned when the job or screenshot was created, used on job reads (GET /jobs/{id}, report, files, cancel). The prepaid key that paid a job is accepted in its place.
  name: jobToken
  scheme: bearer
  sources:
  - openapi/difficat-com-openapi.yml
  type: http
- description: A share token (dcs_…) a snapshot's owner issued in the web app. It reads that one snapshot and starts live compares against it; it never lists, manages or pays.
  key_prefix: dcs_
  name: shareToken
  scheme: bearer
  sources:
  - openapi/difficat-com-openapi.yml
  type: http
- description: The same share token, sent beside a paying Authorization credential on the two compare routes.
  in: header
  name: shareTokenHeader
  parameter: X-DiffiCat-Share
  sources:
  - openapi/difficat-com-openapi.yml
  type: apiKey
slug: difficat-com-authentication
source_filename: difficat-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://difficat.com/llms.txt\ndocs: https://difficat.com/agents\ndocs_additional:\n- https://difficat.com/llms.txt\nderived_from: openapi/difficat-com-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  unauthenticated_allowance: true\n  note: 'No credential is required for the one-time free allowance (40 comparison pages, 5 page\n    discoveries and 5 screenshots per client address). Beyond it a call is paid by prepaid key, Pro\n    account key, or per call over HTTP 402 (Machine Payments Protocol / x402). Keys are only obtained\n    by a signed-in human at https://app.difficat.com/account: \"no call obtains a key without an account\".'\nschemes:\n- name: payment\n  type: http\n  scheme: Payment\n  description: 'Machine Payments Protocol (mpp.dev). A first request without a credential is answered\n    with 402 and a WWW-Authenticate: Payment challenge; the paid retry carries Authorization:\
  \ Payment\n    <credential>. Successful responses carry a Payment-Receipt header. x402 clients are accepted on the\n    same routes for USDC on Base. Over MCP the challenge is JSON-RPC error -32042 and the credential\n    travels in _meta[\"org.paymentauth/credential\"].'\n  sources:\n  - openapi/difficat-com-openapi.yml\n  - https://difficat.com/llms.txt\n- name: prepaidKey\n  type: http\n  scheme: bearer\n  key_prefix: dck_\n  description: 'A prepaid key (dck_…) from the account page at /account, where a signed-in human tops\n    up by card through Stripe Checkout and copies the key. Sent as Authorization: Bearer dck_…; on MCP a\n    gateway that cannot set Authorization may send it as X-DiffiCat-Key. An insufficient balance answers\n    402, an unknown key 401.'\n  alternate_header: X-DiffiCat-Key\n  sources:\n  - openapi/difficat-com-openapi.yml\n  - https://difficat.com/llms.txt\n- name: proKey\n  type: http\n  scheme: bearer\n  description: A Pro account's API key draws on the 5,000\
  \ captured pages a month included in Pro, with\n    overage billed up to a cap set on the account page.\n  sources:\n  - https://difficat.com/llms.txt\n- name: jobToken\n  type: http\n  scheme: bearer\n  description: The one-time jobToken returned when the job or screenshot was created, used on job reads\n    (GET /jobs/{id}, report, files, cancel). The prepaid key that paid a job is accepted in its place.\n  sources:\n  - openapi/difficat-com-openapi.yml\n- name: shareToken\n  type: http\n  scheme: bearer\n  key_prefix: dcs_\n  description: A share token (dcs_…) a snapshot's owner issued in the web app. It reads that one snapshot\n    and starts live compares against it; it never lists, manages or pays.\n  sources:\n  - openapi/difficat-com-openapi.yml\n- name: shareTokenHeader\n  type: apiKey\n  in: header\n  parameter: X-DiffiCat-Share\n  description: The same share token, sent beside a paying Authorization credential on the two compare\n    routes.\n  sources:\n  - openapi/difficat-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/difficat-com/authentication/difficat-com-authentication.yml
summary_line: apiKey/http · 6 schemes
tags:
- Company
- Website Migration
- Visual Regression
- Testing
- QA
- SEO
- MCP
- AI Agents
- x402
---
