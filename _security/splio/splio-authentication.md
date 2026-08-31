---
api_key_in: []
api_specs:
- filename: TzRX9kyT
  format: yaml
  label: Splio Referral API
  slug: splio-referral-api
  spec_type: Postman
  url: https://documenter.getpostman.com/view/10206569/TzRX9kyT
- filename: splio-blacklist-api-openapi.yml
  format: yaml
  label: Splio Blacklist API
  slug: splio-blacklist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splio/refs/heads/main/openapi/splio-blacklist-api-openapi.yml
- filename: splio-contact-api-openapi.yml
  format: yaml
  label: Splio Contact API
  slug: splio-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splio/refs/heads/main/openapi/splio-contact-api-openapi.yml
- filename: splio-coupon-api-openapi.yml
  format: yaml
  label: Splio Coupon API
  slug: splio-coupon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splio/refs/heads/main/openapi/splio-coupon-api-openapi.yml
- filename: splio-export-api-openapi.yml
  format: yaml
  label: Splio Export API
  slug: splio-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splio/refs/heads/main/openapi/splio-export-api-openapi.yml
- filename: splio-fields-api-openapi.yml
  format: yaml
  label: Splio Fields API
  slug: splio-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splio/refs/heads/main/openapi/splio-fields-api-openapi.yml
- filename: splio-filter-api-openapi.yml
  format: yaml
  label: Splio Filter API
  slug: splio-filter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splio/refs/heads/main/openapi/splio-filter-api-openapi.yml
- filename: splio-general-api-openapi.yml
  format: yaml
  label: Splio General API
  slug: splio-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splio/refs/heads/main/openapi/splio-general-api-openapi.yml
- filename: splio-group-api-openapi.yml
  format: yaml
  label: Splio Group API
  slug: splio-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splio/refs/heads/main/openapi/splio-group-api-openapi.yml
- filename: splio-loyalty-api-openapi.yml
  format: yaml
  label: Splio Loyalty API
  slug: splio-loyalty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splio/refs/heads/main/openapi/splio-loyalty-api-openapi.yml
- filename: splio-members-api-openapi.yml
  format: yaml
  label: Splio Members API
  slug: splio-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splio/refs/heads/main/openapi/splio-members-api-openapi.yml
- filename: splio-one-shot-api-openapi.yml
  format: yaml
  label: Splio One Shot API
  slug: splio-one-shot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splio/refs/heads/main/openapi/splio-one-shot-api-openapi.yml
- filename: splio-points-api-openapi.yml
  format: yaml
  label: Splio Points API
  slug: splio-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splio/refs/heads/main/openapi/splio-points-api-openapi.yml
- filename: splio-programs-api-openapi.yml
  format: yaml
  label: Splio Programs API
  slug: splio-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splio/refs/heads/main/openapi/splio-programs-api-openapi.yml
- filename: splio-reward-api-openapi.yml
  format: yaml
  label: Splio Reward API
  slug: splio-reward-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splio/refs/heads/main/openapi/splio-reward-api-openapi.yml
- filename: splio-reward-stock-and-codes-api-openapi.yml
  format: yaml
  label: Splio Reward stock and codes API
  slug: splio-reward-stock-and-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splio/refs/heads/main/openapi/splio-reward-stock-and-codes-api-openapi.yml
- filename: splio-sales-data-api-openapi.yml
  format: yaml
  label: Splio Sales data API
  slug: splio-sales-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splio/refs/heads/main/openapi/splio-sales-data-api-openapi.yml
- filename: splio-universe-api-openapi.yml
  format: yaml
  label: Splio Universe API
  slug: splio-universe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splio/refs/heads/main/openapi/splio-universe-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Splio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Splio secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Splio
provider_slug: splio
scheme_count: 1
schemes:
- bearer_format: JWT
  header: Authorization
  in: header
  minted_by:
    operation: POST /authenticate
    reference: https://dev-scp.splio.com/reference/post_authenticate
    request_fields:
    - api_key
    - password
    spec: openapi/splio-customer-platform-openapi.json
  name: Bearer
  note: The same bearer-JWT model is declared under six different securityScheme names across Splio's six published specs. That is a naming inconsistency in the contracts, not six auth models.
  scheme: bearer
  sources:
  - openapi/splio-customer-platform-openapi.json
  - openapi/splio-campaign-api-openapi.json
  - openapi/splio-campaign-api-v1-openapi.json
  - openapi/splio-content-api-openapi.json
  - openapi/splio-interactions-api-openapi.json
  - openapi/splio-messaging-api-openapi.json
  spec_scheme_names:
  - Bearer
  - Token
  - Authorization
  - bearerAuth
  - BearerAuth
  token_lifetime: 24h
  type: http
  value_format: Bearer xxxxxx.yyyyyyy.zzzzz
slug: splio-authentication
source_filename: splio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://dev-scp.splio.com/reference/authentication-2\ndocs:\n- https://dev-scp.splio.com/reference/authentication-2\n- https://dev-scp.splio.com/docs/authentication-1\n- https://dev-scp.splio.com/reference/post_authenticate\n- https://dev-scp.splio.com/docs/authentication\nsummary:\n  model: api-key-exchanged-for-jwt-bearer\n  types:\n  - http\n  note: >-\n    Every Splio Customer Platform API call carries `Authorization: Bearer <JWT>`. The JWT is not\n    long-lived credential material of its own: it is minted by POSTing an API key to\n    /authenticate and is valid for 24 hours. The API key itself is created and revoked in the\n    universe admin section of the Splio application (www.sp-ring.com).\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  in: header\n  header: Authorization\n  value_format: 'Bearer xxxxxx.yyyyyyy.zzzzz'\n  token_lifetime: 24h\n  minted_by:\n    operation: POST /authenticate\n\
  \    spec: openapi/splio-customer-platform-openapi.json\n    reference: https://dev-scp.splio.com/reference/post_authenticate\n    request_fields:\n    - api_key\n    - password\n  sources:\n  - openapi/splio-customer-platform-openapi.json\n  - openapi/splio-campaign-api-openapi.json\n  - openapi/splio-campaign-api-v1-openapi.json\n  - openapi/splio-content-api-openapi.json\n  - openapi/splio-interactions-api-openapi.json\n  - openapi/splio-messaging-api-openapi.json\n  spec_scheme_names:\n  - Bearer      # splio-customer-platform, splio-interactions-api\n  - Token       # splio-campaign-api\n  - Authorization  # splio-campaign-api-v1\n  - bearerAuth  # splio-messaging-api\n  - BearerAuth  # splio-content-api\n  note: >-\n    The same bearer-JWT model is declared under six different securityScheme names across Splio's\n    six published specs. That is a naming inconsistency in the contracts, not six auth models.\ncredentials:\n- name: API key\n  where: Splio universe admin -> API users\
  \ list\n  docs: https://dev-scp.splio.com/docs/authentication-1\n  provisioning: administrator-issued (no self-serve developer signup)\n  rotation: managed in the universe admin section\n  guidance_from_provider:\n  - Use one API key per connecting system (e-commerce, PoS, ...) so a system can be identified during\n    an investigation.\n  - Do not re-authenticate on every call; the JWT is valid for 24 hours.\n  - Never share the API key, including with Splio Customer Care — the last 3 characters plus the\n    universe name are sufficient for support.\n- name: Referral API token\n  scheme: sha256-hmac-like digest\n  docs: https://documenter.getpostman.com/view/10206569/TzRX9kyT\n  note: >-\n    The separately published Splio Referral API does NOT use the JWT model. It authenticates by\n    SHA-256 hashing the concatenation of the coupon code and a key issued by the Splio project\n    manager, passed as form-data in the request body.\nsso:\n  supported: true\n  scope: application users\
  \ (not API callers)\n  docs: https://dev-scp.splio.com/docs/authentication\n  note: SAML/SSO is available for logging human users into the Splio application, separate from API auth.\noauth2:\n  supported: false\n  note: >-\n    No oauth2 or openIdConnect securityScheme appears in any published Splio spec, and no\n    /.well-known/oauth-authorization-server or /.well-known/openid-configuration document is served\n    on splio.com, api.splio.com or dev-scp.splio.com. scopes/ is therefore not applicable.\nmutual_tls:\n  supported: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/splio/refs/heads/main/authentication/splio-authentication.yml
summary_line: http · 1 scheme
tags:
- marketing-automation
- customer-data-platform
- loyalty
- CRM
- email-marketing
- SMS
- mobile-wallet
- Retail
- E-Commerce
- predictive-ai
- Customer Engagement
- france
---
