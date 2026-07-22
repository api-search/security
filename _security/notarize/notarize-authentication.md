---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Notarize Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Notarize secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Notarize
provider_slug: notarize
scheme_count: 2
schemes:
- description: 'Static API key sent in the `ApiKey` request header. Two access levels are issued: Full Access (create/update/delete transactions; secret, server-side only) and Client Only (create transactions only; safe to expose in client-facing apps, powers EasyLinks).'
  docs: https://dev.proof.com/docs/api-keys
  in: header
  key_prefixes:
    client_only_fairfax: prf_cli_test_
    client_only_production: prf_cli_
    full_access_fairfax: prf_test_
    full_access_production: prf_
  name: ApiKey
  parameter_name: ApiKey
  secret_scanning: Proof partners with GitHub Secret Scanning; leaked keys are detected and should be revoked immediately.
  type: apiKey
- description: 'OAuth 2.0 client_credentials grant as an alternative to API keys. Client apps are provisioned under Settings > OAuth; client_id/client_secret are passed via HTTP Basic auth to the token endpoint. Access tokens are Bearer tokens (expires_in 7200s / 2h). Requires `Content-Type: application/x-www-form-urlencoded` (else HTTP 415).'
  docs: https://dev.proof.com/docs/oauth-client-credentials
  flows:
  - expires_in: 7200
    flow: clientCredentials
    scopes:
      read: Read access
      write: Write access
    tokenUrl: https://api.proof.com/oauth/v2/token
    tokenUrl_fairfax: https://api.fairfax.proof.com/oauth/v2/token
    token_info_url: https://api.proof.com/oauth/v2/token/info
    token_type: Bearer
  name: OAuth2
  type: oauth2
slug: notarize-authentication
source_filename: notarize-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://dev.proof.com/docs/api-keys\ndocs:\n  - https://dev.proof.com/docs/api-keys\n  - https://dev.proof.com/docs/oauth-client-credentials\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  api_key_header: ApiKey\n  oauth2_flows: [clientCredentials]\nschemes:\n  - name: ApiKey\n    type: apiKey\n    in: header\n    parameter_name: ApiKey\n    description: >-\n      Static API key sent in the `ApiKey` request header. Two access levels are\n      issued: Full Access (create/update/delete transactions; secret, server-side\n      only) and Client Only (create transactions only; safe to expose in\n      client-facing apps, powers EasyLinks).\n    key_prefixes:\n      full_access_production: prf_\n      full_access_fairfax: prf_test_\n      client_only_production: prf_cli_\n      client_only_fairfax: prf_cli_test_\n    secret_scanning: >-\n      Proof partners with GitHub Secret Scanning; leaked keys are detected and\n\
  \      should be revoked immediately.\n    docs: https://dev.proof.com/docs/api-keys\n  - name: OAuth2\n    type: oauth2\n    description: >-\n      OAuth 2.0 client_credentials grant as an alternative to API keys. Client\n      apps are provisioned under Settings > OAuth; client_id/client_secret are\n      passed via HTTP Basic auth to the token endpoint. Access tokens are Bearer\n      tokens (expires_in 7200s / 2h). Requires\n      `Content-Type: application/x-www-form-urlencoded` (else HTTP 415).\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://api.proof.com/oauth/v2/token\n        tokenUrl_fairfax: https://api.fairfax.proof.com/oauth/v2/token\n        token_info_url: https://api.proof.com/oauth/v2/token/info\n        token_type: Bearer\n        expires_in: 7200\n        scopes:\n          read: Read access\n          write: Write access\n    docs: https://dev.proof.com/docs/oauth-client-credentials\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/authentication/notarize-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Proptech
- Notarization
- Remote Online Notarization
- Identity Verification
- eSignature
- Digital Credentials
- Real Estate
- Mortgage
- Legal Tech
---
