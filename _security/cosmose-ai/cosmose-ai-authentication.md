---
api_key_in: []
api_specs:
- filename: cosmose-ai-contact-form-controller-api-openapi.yml
  format: yaml
  label: Cosmose AI Contact Form Controller API
  slug: cosmose-ai-contact-form-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmose-ai/refs/heads/main/openapi/cosmose-ai-contact-form-controller-api-openapi.yml
- filename: cosmose-ai-crucible-token-controller-api-openapi.yml
  format: yaml
  label: Cosmose AI Crucible Token Controller API
  slug: cosmose-ai-crucible-token-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmose-ai/refs/heads/main/openapi/cosmose-ai-crucible-token-controller-api-openapi.yml
- filename: cosmose-ai-forget-me-controller-api-openapi.yml
  format: yaml
  label: Cosmose AI Forget Me Controller API
  slug: cosmose-ai-forget-me-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmose-ai/refs/heads/main/openapi/cosmose-ai-forget-me-controller-api-openapi.yml
- filename: cosmose-ai-invitation-controller-api-openapi.yml
  format: yaml
  label: Cosmose AI Invitation Controller API
  slug: cosmose-ai-invitation-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmose-ai/refs/heads/main/openapi/cosmose-ai-invitation-controller-api-openapi.yml
- filename: cosmose-ai-kkn-onboarding-controller-api-openapi.yml
  format: yaml
  label: Cosmose AI Kkn Onboarding Controller API
  slug: cosmose-ai-kkn-onboarding-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmose-ai/refs/heads/main/openapi/cosmose-ai-kkn-onboarding-controller-api-openapi.yml
- filename: cosmose-ai-learn-to-code-controller-api-openapi.yml
  format: yaml
  label: Cosmose AI Learn To Code Controller API
  slug: cosmose-ai-learn-to-code-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmose-ai/refs/heads/main/openapi/cosmose-ai-learn-to-code-controller-api-openapi.yml
- filename: cosmose-ai-merchant-controller-api-openapi.yml
  format: yaml
  label: Cosmose AI Merchant Controller API
  slug: cosmose-ai-merchant-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmose-ai/refs/heads/main/openapi/cosmose-ai-merchant-controller-api-openapi.yml
- filename: cosmose-ai-newsletter-controller-api-openapi.yml
  format: yaml
  label: Cosmose AI Newsletter Controller API
  slug: cosmose-ai-newsletter-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmose-ai/refs/heads/main/openapi/cosmose-ai-newsletter-controller-api-openapi.yml
- filename: cosmose-ai-onboarding-controller-api-openapi.yml
  format: yaml
  label: Cosmose AI Onboarding Controller API
  slug: cosmose-ai-onboarding-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmose-ai/refs/heads/main/openapi/cosmose-ai-onboarding-controller-api-openapi.yml
- filename: cosmose-ai-registration-admin-controller-api-openapi.yml
  format: yaml
  label: Cosmose AI Registration Admin Controller API
  slug: cosmose-ai-registration-admin-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmose-ai/refs/heads/main/openapi/cosmose-ai-registration-admin-controller-api-openapi.yml
- filename: cosmose-ai-registration-controller-api-openapi.yml
  format: yaml
  label: Cosmose AI Registration Controller API
  slug: cosmose-ai-registration-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmose-ai/refs/heads/main/openapi/cosmose-ai-registration-controller-api-openapi.yml
- filename: cosmose-ai-school-controller-api-openapi.yml
  format: yaml
  label: Cosmose AI School Controller API
  slug: cosmose-ai-school-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmose-ai/refs/heads/main/openapi/cosmose-ai-school-controller-api-openapi.yml
- filename: cosmose-ai-token-controller-api-openapi.yml
  format: yaml
  label: Cosmose AI Token Controller API
  slug: cosmose-ai-token-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmose-ai/refs/heads/main/openapi/cosmose-ai-token-controller-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cosmose Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cosmose AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cosmose AI
provider_slug: cosmose-ai
scheme_count: 1
schemes:
- applied: global
  bearerFormat: JWT
  detail: 'Declared once in components.securitySchemes and applied at the document root (`security: [{bearerAuth: []}]`), so every one of the 24 operations inherits it — including the public-facing lead-capture endpoints (/v1/contact-forms, /v1/newsletter, /v1/merchants, /v1/schools) that the marketing site posts to from an unauthenticated browser. The contract therefore over-declares auth relative to observed behaviour; the spec does not distinguish the anonymous endpoints from the authenticated ones.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cosmose-ai-deal-hunter-registration-api-openapi.yml
  type: http
slug: cosmose-ai-authentication
source_filename: cosmose-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: derived\nsource: openapi/cosmose-ai-deal-hunter-registration-api-openapi.yml\nnote: >-\n  Derived from the provider's own published OpenAPI plus observed live gateway responses. Cosmose AI publishes no\n  developer authentication documentation — there is no developer portal, no API reference page and no key-issuance\n  flow a member of the public can reach — so everything below comes from the contract and from probing.\nsummary:\n  types:\n  - http\n  primary: bearer JWT\n  scheme_count: 1\n  applied_globally: true\n  developer_docs_published: false\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applied: global\n  detail: >-\n    Declared once in components.securitySchemes and applied at the document root (`security: [{bearerAuth: []}]`), so\n    every one of the 24 operations inherits it — including the public-facing lead-capture endpoints\n    (/v1/contact-forms, /v1/newsletter, /v1/merchants, /v1/schools)\
  \ that the marketing site posts to from an\n    unauthenticated browser. The contract therefore over-declares auth relative to observed behaviour; the spec does\n    not distinguish the anonymous endpoints from the authenticated ones.\n  sources:\n  - openapi/cosmose-ai-deal-hunter-registration-api-openapi.yml\ntoken_endpoints:\n- operationId: generateTokens\n  method: POST\n  path: /v2/token\n  description: >-\n    OAuth-2-shaped but not OAuth 2.0 — parameters are named `grant_type` (required), `refresh_token` and `scope`\n    (default value `kaikai`), yet they are carried as QUERY parameters rather than an\n    application/x-www-form-urlencoded body, no securityScheme of type oauth2 is declared, and no authorization or\n    discovery endpoint is published. Returns a TokenInfo object with `access_token`, `refresh_token`, `type` and\n    `expires_in`.\n  additional_inputs:\n  - name: Installation-Id\n    in: header\n    detail: Device/installation identifier, optional in the contract,\
  \ used to bind tokens to an app installation.\n- operationId: generateTokens_1\n  method: POST\n  path: /v2/crucible-token\n  description: >-\n    Second token issuer under an internal product codename (\"crucible\"), same TokenInfo response shape. Undocumented\n    publicly; its relationship to /v2/token is not described in the contract.\noauth2:\n  declared: false\n  discovery:\n    openid_configuration: false\n    oauth_authorization_server: false\n  note: >-\n    Probed /.well-known/openid-configuration and /.well-known/oauth-authorization-server on cosmose.ai, cosmose.co,\n    kaikai.ai, api.cosmose.co, api.sg.cosmose.co and repo.cosmose.co on 2026-08-11. The web hosts answer HTTP 200\n    with the Angular single-page-app shell for every path (byte-identical to the homepage — a soft 200, not a\n    document); the API gateways answer 401; repo.cosmose.co answers 404. No discovery document exists.\ngateway_behaviour:\n  probed: '2026-08-11'\n  observations:\n  - host: api.cosmose.co\n\
  \    path: /\n    status: 401\n    body: '{\"error\":\"unauthorized\",\"error_description\":\"Full authentication is required to access this resource\"}'\n  - host: api.sg.cosmose.co\n    path: /\n    status: 401\n    body: '{\"error\":\"unauthorized\",\"error_description\":\"Full authentication is required to access this resource\"}'\n  - host: api.sg.cosmose.co\n    path: /deal-hunter-registration-api/v3/api-docs\n    status: 200\n    body: OpenAPI 3.0.1 document, served anonymously\n  note: >-\n    The gateway's own 401 envelope (`error` / `error_description`) is a different error shape from the ErrorDto\n    (`errorCode` / `message`) the service returns, and neither 401 nor the gateway envelope appears anywhere in the\n    published contract. See errors/cosmose-ai-problem-types.yml.\nkey_issuance:\n  self_serve: false\n  documented: false\n  detail: >-\n    No signup, no console, no key request form was found on any Cosmose AI or KaiKai property. Access appears to be\n    partner-provisioned;\
  \ the iOS SDK distribution repository (repo.cosmose.co) also requires credentials — a\n    directory listing of /repository/ios-sdk-releases/ returned 401 on 2026-08-11.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cosmose-ai/refs/heads/main/authentication/cosmose-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- retail-intelligence
- offline-analytics
- location-intelligence
- adtech
- consumer-behavior
- shopper-analytics
- mobile-sdk
- Advertising
- artificial-intelligence
- singapore
---
