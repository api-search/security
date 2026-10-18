---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Bolttech Authentication
name_suffix: Authentication
oauth_flows: []
overview: bolttech declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: bolttech
provider_slug: bolttech
scheme_count: 1
schemes:
- credential_lifecycle: To rotate compromised credentials, delete the app and create a new one with the same API.
  description: Issued per app after creating an app ("+ New App") in the developer portal account; entered via the "Authorize" button on each API documentation page. The docs state calls carry an access token. Exact token flow is documented only inside the login-gated Apigee portal catalogue.
  name: API key and secret (client ID / client secret)
  type: apiKey
slug: bolttech-authentication
source_filename: bolttech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: searched\nsource:\n- https://developers.bolttech.io/get-started\n- https://developers.bolttech.io/faqs\ndocs: https://developers.bolttech.io/get-started\nschemes:\n- type: apiKey\n  name: API key and secret (client ID / client secret)\n  description: Issued per app after creating an app (\"+ New App\") in the developer portal account; entered via the \"Authorize\" button on each API documentation page. The docs state calls carry an access token. Exact token flow is documented only inside the login-gated Apigee portal catalogue.\n  credential_lifecycle: To rotate compromised credentials, delete the app and create a new one with the same API.\nsummary: Self-service registration on developers.bolttech.io (Apigee integrated portal) issues sandbox API key + secret per app; production access by email to dev-bolttechex-api@bolttech.io. The API catalogue and specs are gated behind login.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bolttech/refs/heads/main/authentication/bolttech-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Insurance
- Embedded Insurance
- Insurtech
---
