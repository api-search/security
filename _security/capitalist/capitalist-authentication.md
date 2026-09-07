---
anonymous_access: false
api_key_in: []
api_specs:
- filename: capitalist-integration-api-openapi.json
  format: json
  label: Capitalist API
  slug: capitalist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capitalist/refs/heads/main/openapi/capitalist-integration-api-openapi.json
- filename: capitalist-capitalist-payments-api-api-openapi.yml
  format: yaml
  label: Capitalist Payments API (v1, deprecated)
  slug: capitalist-capitalist-payments-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capitalist/refs/heads/main/openapi/capitalist-capitalist-payments-api-api-openapi.yml
auth_types: []
description: 'Capitalist runs two authentication models side by side. The current Integration API (v2, https://api2.capitalist.net) uses a three-header signed-request scheme: an API key, a millisecond epoch timestamp, and a SHA-256 hex signature over the timestamp, the raw request body and the API secret. The deprecated v1 API (https://api.capitalist.net) authenticates with the account login plus either a plain password, an encrypted password or a certificate signature carried as form fields. Neither surface uses OAuth, and no /.well-known/openid-configuration or oauth-authorization-server document is served on any Capitalist host (all probed 404 on 2026-09-05).'
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Capitalist Authentication
name_suffix: Authentication
oauth_flows: []
overview: Capitalist declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Capitalist
provider_slug: capitalist
scheme_count: 0
schemes: []
slug: capitalist-authentication
source_filename: capitalist-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: >-\n  https://docs.capitalist.net/api/integration-api.html sections 2 (Authentication),\n  2.2 (Signature Calculation Example) and 3 (Security: IP Whitelist), cross-checked\n  against the first-party OpenAPI at\n  https://github.com/capitalist-net/API-V2/blob/main/java-client/api-definition/Integration+API.json\n  and a live anonymous probe of https://api2.capitalist.net/v1/rate (HTTP 401,\n  body \"Missing `API-Key`\", observed 2026-09-05).\nprovider: Capitalist\nproviderId: capitalist\ndescription: >-\n  Capitalist runs two authentication models side by side. The current\n  Integration API (v2, https://api2.capitalist.net) uses a three-header\n  signed-request scheme: an API key, a millisecond epoch timestamp, and a\n  SHA-256 hex signature over the timestamp, the raw request body and the API\n  secret. The deprecated v1 API (https://api.capitalist.net) authenticates with\n  the account login plus either a plain password,\
  \ an encrypted password or a\n  certificate signature carried as form fields. Neither surface uses OAuth, and\n  no /.well-known/openid-configuration or oauth-authorization-server document is\n  served on any Capitalist host (all probed 404 on 2026-09-05).\n\napis:\n  - name: Capitalist Integration API (v2)\n    base_url: https://api2.capitalist.net\n    status: current\n    docs: https://docs.capitalist.net/api/integration-api.html\n    schemes:\n      - id: api-key-signed\n        type: apiKey\n        in: header\n        name: API-Key\n        description: >-\n          API key generated in the account's Security section\n          (https://capitalist.net/security). The provider's docs state that API\n          access must be enabled and Google 2FA activated on the account before\n          a key can be created.\n      - id: request-timestamp\n        type: apiKey\n        in: header\n        name: X-Request-Timestamp\n        description: Current timestamp in epoch milliseconds; also\
  \ the anti-replay nonce.\n      - id: request-signature\n        type: apiKey\n        in: header\n        name: Signature\n        description: >-\n          sha256_hex(X-Request-Timestamp + raw request body + API secret), sent\n          as a lowercase hex string. All three headers are required on every\n          call.\n    signing:\n      algorithm: SHA-256\n      encoding: hex\n      formula: 'Signature = sha256_hex(X-Request-Timestamp + request_body + API-secret)'\n      secret: API secret, issued alongside the API key in the account Security section\n      replay_protection: >-\n        The signature covers X-Request-Timestamp, so a captured request cannot be\n        replayed with a different timestamp. The docs do not state a clock-skew\n        tolerance window.\n      docs: https://docs.capitalist.net/api/integration-api.html\n    callback_verification:\n      description: >-\n        Outbound payment and KYC callbacks are signed with the SAME construction:\n        the provider\
  \ sends X-Request-Timestamp and Signature headers, and the\n        integrator recomputes sha256_hex(timestamp + body + API secret) to verify\n        authenticity.\n      headers: [X-Request-Timestamp, Signature]\n      docs: https://docs.capitalist.net/api/integration-api.html\n    network_controls:\n      ip_allowlist:\n        supported: true\n        description: >-\n          API methods may be restricted to an allowlist of IP addresses; requests\n          from IPs outside the list are rejected. Exact IPs and last-octet\n          wildcards (e.g. 127.0.0.*) are accepted.\n        endpoints:\n          - GET /v1/whitelist\n          - POST /v1/whitelist\n          - POST /v1/whitelist/remove\n        docs: https://docs.capitalist.net/api/integration-api.html\n    account_prerequisites:\n      - API access enabled on the account\n      - Google Authenticator (2FA) activated on the account\n      - API key and API secret created at https://capitalist.net/security\n    live_probe:\n\
  \      url: https://api2.capitalist.net/v1/rate?from=USD&to=EUR\n      status: 401\n      body: 'Missing `API-Key`'\n      checked: '2026-09-05'\n\n  - name: Capitalist Payments API (v1, deprecated)\n    base_url: https://api.capitalist.net\n    status: deprecated\n    docs: https://capitalist.net/developers/deprecated/v1/api\n    schemes:\n      - id: form-credentials\n        type: apiKey\n        in: formData\n        name: login\n        description: Capitalist account username (not the account email), sent as a form field.\n      - id: form-password\n        type: apiKey\n        in: formData\n        name: password\n        description: >-\n          Plain password, an encrypted password, or a certificate-derived\n          signature depending on the operation's verification level. The\n          provider publishes PHP and Java reference implementations of the\n          encryption and signing at https://github.com/capitalist-net.\n      - id: one-time-token\n        type: apiKey\n\
  \        in: formData\n        name: token\n        description: One-time security token obtained via the get_token operation.\n    live_probe:\n      url: https://api.capitalist.net/\n      status: 200\n      note: >-\n        GET returns 150;\"Received a non-POST request. (API version 1.9.8)\".\n        A POST without the x-response-format header returns\n        {\"code\":4,\"message\":\"Only x-response-format=json is available.\"}; with\n        the header it returns a validation error naming login, encrypted_password\n        and token as required. Probed anonymously 2026-09-05.\n      checked: '2026-09-05'\n\noauth:\n  supported: false\n  note: >-\n    No OAuth 2.0 or OpenID Connect surface. /.well-known/openid-configuration\n    and /.well-known/oauth-authorization-server return 404 on capitalist.net,\n    api.capitalist.net and api2.capitalist.net (probed 2026-09-05). There is\n    therefore no scopes/ artifact for this provider.\n\nmtls:\n  supported: false\n  note: >-\n    v1\
  \ uses client-held certificates to SIGN request payloads (see\n    https://github.com/capitalist-net/Capitalist-API-Java-crypto), not for\n    transport-layer mutual TLS.\n\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capitalist/refs/heads/main/authentication/capitalist-authentication.yml
summary_line: 0 schemes
tags:
- Bulk Payouts
- Cryptocurrency
- Finance
- Mass Payments
- Payment Platform
- Payments
- Payouts
- Remittance
---
