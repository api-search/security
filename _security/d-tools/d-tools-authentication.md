---
api_key_in: []
api_specs:
- filename: d-tools-cloud-api-openapi.yml
  format: yaml
  label: D-Tools Cloud API
  slug: d-tools-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-tools/refs/heads/main/openapi/d-tools-cloud-api-openapi.yml
- filename: d-tools-si-api-openapi.yml
  format: yaml
  label: D-Tools System Integrator (SI) API
  slug: d-tools-system-integrator-si-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-tools/refs/heads/main/openapi/d-tools-si-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: D Tools Authentication
name_suffix: Authentication
oauth_flows: []
overview: D-Tools declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: D-Tools
provider_slug: d-tools
scheme_count: 0
schemes: []
slug: d-tools-authentication
source_filename: d-tools-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: searched\nsource: >-\n  https://docs.d-tools.cloud/en/articles/8756132-authentication ,\n  https://docs.d-tools.cloud/en/articles/8756116-api-keys-and-webhooks ,\n  https://api.d-tools.com/si/openapi/v1.json (info.description) ,\n  https://docs.d-tools.com/en/articles/9225625-d-tools-si-api-overview\nspec_gap: >-\n  NEITHER OpenAPI declares components.securitySchemes and neither declares a root-level `security` block. Both APIs\n  are in fact authenticated on every operation, but a generated client or an agent reading either contract alone\n  would produce unauthenticated calls that fail 401. The auth model below is recovered from the prose docs, not\n  from the machine-readable contract. This is the single largest contract defect in the D-Tools surface and it is\n  the provider's to fix: adding `securitySchemes` with an `apiKey`-in-header scheme plus a root `security` block\n  costs a few lines and makes both specs self-describing.\napis:\n\
  - api: D-Tools Cloud API\n  base_url: https://dtcloudapi.d-tools.cloud\n  model: dual-credential\n  note: >-\n    Both credentials are required on every request; supplying only one returns 401. The Basic value is a single\n    fixed string that D-Tools publishes verbatim in its own public documentation and instructs every customer to\n    reuse (\"Do not make your own, as it will not work\"), so it is a shared, non-rotatable, non-secret constant\n    rather than a per-tenant credential. The only tenant-specific credential is the X-API-Key. That value is\n    deliberately NOT reproduced in this artifact.\n  schemes:\n  - name: api_key\n    type: apiKey\n    in: header\n    header: X-API-Key\n    scope: per-tenant\n    issued_via: 'D-Tools Cloud app: Settings > Integration > Developer > API Keys'\n    rotation: manual; keys can be edited to inactive or deleted from the same screen\n    max_active_keys: 5\n    docs: https://docs.d-tools.cloud/en/articles/8756116-api-keys-and-webhooks\n  -\
  \ name: shared_basic\n    type: http\n    scheme: basic\n    in: header\n    header: Authorization\n    scope: shared-global\n    rotation: none documented\n    docs: https://docs.d-tools.cloud/en/articles/8756132-authentication\n    observation: >-\n      A fixed Basic credential published in public docs and identical for every customer. It adds no tenant\n      separation; the X-API-Key carries all of the actual authorization. Recorded as a finding, not as a secret.\n  failure_mode: 401 Unauthorized, body shaped as ASP.NET Core ProblemDetails\n  oauth2: false\n  openid_connect: false\n  mtls: false\n- api: D-Tools System Integrator (SI) API\n  base_url: https://api.d-tools.com/si\n  model: single-credential\n  schemes:\n  - name: api_key\n    type: apiKey\n    in: header\n    header: X-DTSI-ApiKey\n    scope: per SI user AND per integration\n    issued_via: 'SI 2016 Control Panel > Manage Integrations'\n    rotation: not documented\n    docs: https://docs.d-tools.com/en/articles/9203156-api-key\n\
  \    note: >-\n      One key binds one integration to one SI user, so a partner integrating with N SI customers holds N keys.\n      Access to the SI API is gated on enrollment in the D-Tools Software Assurance (SA) program.\n  oauth2: false\n  openid_connect: false\n  mtls: false\nend_user_identity:\n  sso: >-\n    Product-level only, not API-level. D-Tools Cloud sign-in uses Microsoft Entra External ID with MFA; SI supports\n    a Microsoft Entra ID integration. Neither is exposed to API consumers — there is no authorization-code flow, no\n    consent screen, and no delegated end-user token on either API.\n  delegated_authorization: false\n  scopes: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/d-tools/refs/heads/main/authentication/d-tools-authentication.yml
summary_line: 0 schemes
tags:
- av-integration
- Systems Integration
- Project Management
- Estimation
- Quoting
- Field Service Management
- Construction Tech
- low-voltage
- Product Catalog
- ERP Integration
- Vertical SaaS
---
