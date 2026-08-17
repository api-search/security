---
api_key_in:
- header
api_specs:
- filename: owler-enterprise-api-openapi.yml
  format: yaml
  label: Owler Enterprise API
  slug: owler-enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/owler/refs/heads/main/openapi/owler-enterprise-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Owler Authentication
name_suffix: Authentication
oauth_flows: []
overview: Owler secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Owler
provider_slug: owler
scheme_count: 1
schemes:
- application_style: 'Per-operation. Each operation carries `security: [{api_key: []}]`; the document declares no top-level `security` block, so there is no default and no anonymous operation.'
  applied_to: all 6 operations
  in: header
  name: api_key
  parameter: x-api-key
  sources:
  - openapi/owler-enterprise-api-openapi.yml
  type: apiKey
slug: owler-authentication
source_filename: owler-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: openapi/owler-enterprise-api-openapi.yml\ndocs: https://developers.owler.com/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  scopes: 0\n  credential_count: 1\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/owler-enterprise-api-openapi.yml\n  applied_to: all 6 operations\n  application_style: >-\n    Per-operation. Each operation carries `security: [{api_key: []}]`; the document declares no\n    top-level `security` block, so there is no default and no anonymous operation.\nmodel:\n  single_credential: true\n  scopes: false\n  oauth: false\n  oidc: false\n  mtls: false\n  signing: false\n  rotation_documented: false\n  expiry_documented: false\n  note: >-\n    One long-lived static key in one header. Nothing narrows it: no scopes, no per-product token,\n    no read/write distinction (there is no write path), no expiry, no documented\
  \ rotation\n    procedure, and no way for a caller to introspect what its own key is entitled to.\nprovisioning:\n  self_serve: false\n  url: https://corp.owler.com/data-licensing\n  process: >-\n    Keys are issued by an Owler representative as part of a data-licensing agreement. There is no\n    signup form, no developer dashboard and no key-management UI on developers.owler.com — the\n    portal is a bare Swagger UI with an Authorize box and nothing behind it. Third-party\n    integration guides for Owler (for example Domo's connector documentation) likewise instruct\n    users to obtain the key from their Owler representative.\n  test_credentials: none\nfailure_semantics:\n  status: 403\n  description: Authentication Failed\n  has_401: false\n  note: >-\n    Owler declares NO 401 anywhere in the contract. A missing key, a malformed key, a revoked key\n    and a valid key that is not licensed for the product being called all return the same 403 with\n    no documented body. Because\
  \ Company Premium, Competitor Premium and Feed are separately\n    licensed, this collapses two operationally different conditions — \"fix your credential\" and\n    \"buy this product\" — into one indistinguishable response.\n  challenge_header: none documented\ntransport_security:\n  https_only: true\n  base_url: https://apiv2.owler.com\n  tls_version_observed: TLSv1.3\n  hsts_observed: false\n  hsts_note: >-\n    apiv2.owler.com returned no Strict-Transport-Security header on probe (2026-08-14). The key\n    travels in a plaintext request header, so HSTS on the API host would be a cheap hardening win.\n  edge: AWS API Gateway (unmatched routes return 403 \"Missing Authentication Token\")\n  see: security/owler-domain-security.yml\ndiscovery:\n  oauth_authorization_server: not served (probed on all Owler hosts, no document)\n  openid_configuration: not served (probed on all Owler hosts, no document)\n  see: well-known/owler-well-known.yml\nclient_guidance:\n- Send `x-api-key` on every\
  \ request; there is no operation that works without it.\n- Treat 403 as terminal, never retryable. Do not loop on it — you cannot tell a bad key from an\n  unlicensed product, and retrying fixes neither.\n- Store the key as a secret with no assumed expiry, and arrange rotation with the Owler account\n  team out of band, because no rotation endpoint or policy exists.\n- Do not expect a scope or entitlement claim to inspect; if you need to know what a key covers, the\n  only reliable method is to call one operation per product and observe which return 403.\nscopes_artifact: null\nscopes_note: >-\n  No scopes/ artifact was written. derive-oauth-scopes.py found zero oauth2 schemes and zero scopes\n  across the repo's specs — Owler is a key-auth provider with no scope surface, so an empty scopes\n  file would be noise rather than data.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/owler/refs/heads/main/authentication/owler-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Company Intelligence
- Sales Intelligence
- Competitive Intelligence
- Business Data
- Data Licensing
- News Monitoring
- Market Research
- Firmographics
- Company Search
- Funding Data
---
