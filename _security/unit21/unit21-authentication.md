---
api_key_in: []
auth_types: []
description: Unit21 authenticates every API request with a static organization-scoped API key sent in a custom u21-key request header over HTTPS. There is no OAuth 2.0 authorization server, no OpenID Connect discovery document and no scope surface -- so scopes/ is deliberately not emitted for this provider. An optional second layer encrypts the request payload itself with a Fernet key supplied in a u21-fernet header.
kind: authentication
layout: security
method: searched
name: Unit21 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unit21 declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Unit21
provider_slug: unit21
scheme_count: 0
schemes: []
slug: unit21-authentication
source_filename: unit21-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: https://docs.unit21.ai/reference/generate-api-keys\ndescription: >-\n  Unit21 authenticates every API request with a static organization-scoped API\n  key sent in a custom u21-key request header over HTTPS. There is no OAuth 2.0\n  authorization server, no OpenID Connect discovery document and no scope\n  surface -- so scopes/ is deliberately not emitted for this provider. An\n  optional second layer encrypts the request payload itself with a Fernet key\n  supplied in a u21-fernet header.\nprovenance_note: >-\n  As of 2026-08-27 every page on docs.unit21.ai returns a 7,947-byte\n  \"Sign in | Unit21\" HTML gate to an unauthenticated fetch, so the field values\n  below were read from the public search index of those same pages rather than\n  fetched directly, and corroborated against a live probe of the API host. They\n  are recorded as searched, not probed. Anything that could not be corroborated\n  is left null rather than\
  \ guessed.\nsecurity_schemes:\n  - id: u21-key\n    type: apiKey\n    in: header\n    name: u21-key\n    description: >-\n      Organization-scoped API key. Required on every request; unauthenticated\n      requests fail.\n    scopes: []\n    docs: https://docs.unit21.ai/reference/generate-api-keys\n  - id: u21-fernet\n    type: apiKey\n    in: header\n    name: u21-fernet\n    description: >-\n      Optional payload-encryption key header. When used, the request body is\n      encrypted with Fernet (128-bit AES in CBC mode with PKCS7 padding,\n      authenticated with HMAC-SHA256). Available on all API endpoints.\n    optional: true\n    docs: https://docs.unit21.ai/reference/encryption\noauth2: false\nopenid_connect: false\nmutual_tls: null\nkey_management:\n  self_service: true\n  where: >-\n    Unit21 Dashboard -> Data Management -> Integrations tab -> \"Request a new\n    key\". Administrator privileges required.\n  max_active_keys: 10\n  displayed_once: true\n  stored_by_provider:\
  \ false\n  rotation_guidance: Unit21 recommends rotating keys every 2-6 months.\n  docs: https://docs.unit21.ai/reference/generate-api-keys\ntransport:\n  https_required: true\n  observed:\n    url: https://sandbox1-api.unit21.com/v1/entities/list\n    method: POST\n    status: 401\n    body: '{\"error_code\":\"unauthorized\"}'\n    server: awselb/2.0\n    www_authenticate: null\n    note: >-\n      Probed 2026-08-27 without credentials. The edge returns a bare JSON 401\n      with no WWW-Authenticate challenge, so an agent gets no machine-readable\n      hint about which credential to present.\nenvironments:\n  - name: Sandbox\n    baseURL: https://sandbox1-api.unit21.com/v1\n  - name: Production\n    baseURL: https://{org_name}-api.unit21.com/v1\n    templated: true\n    note: >-\n      The production host is organization-specific and is issued at onboarding;\n      the templated form is the real, correct base and is not a placeholder.\ngaps:\n  - No WWW-Authenticate header on 401, so\
  \ the auth scheme is not discoverable at runtime.\n  - No /.well-known/openid-configuration or /.well-known/oauth-authorization-server (both 404/401).\n  - The authentication reference itself is behind an email sign-in gate.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unit21/refs/heads/main/authentication/unit21-authentication.yml
summary_line: 0 schemes
tags:
- Fraud Detection
- AML
- Anti-Money Laundering
- Compliance
- Fintech
- Transaction Monitoring
- Risk
- SAR
- Financial Crime
- Suspicious Activity Reports
---
