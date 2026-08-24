---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Layerx Authentication
name_suffix: Authentication
oauth_flows: []
overview: LayerX declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: LayerX
provider_slug: layerx
scheme_count: 1
schemes:
- description: 'A tenant-scoped API key issued from the Bakuraku admin console. Per the integrator setup reference the flow is: Bakuraku 管理画面 → API管理 → 新規作成 → select the permissions the key should carry → issue the key. Article 4 of the API terms states LayerX issues "API認証情報" to an approved "API契約者" and that the contract holder bears full responsibility for its safekeeping; the credential may be shared with the contract holder''s own end users but never transferred, lent or sold to third parties.'
  header: unknown
  id: bakuraku-api-key
  in: unknown
  issued_to: An "API契約者" — a legal entity LayerX has approved for API use by its prescribed application process. An existing Bakuraku subscription is a precondition (API terms, Article 3).
  label: Bakuraku API key
  name: unknown
  rotation: LayerX may suspend or re-issue API credentials without the contract holder's consent while an incident is being contained (API terms, Article 6.5).
  type: apiKey
slug: layerx-authentication
source_filename: layerx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: searched\nsource: >-\n  https://bakuraku.jp/terms/api-terms/ (LayerX's own \"バクラクAPI\"利用規約, Articles 4-6),\n  https://bakuraku.jp/workflow/function/api/, https://bakuraku.jp/news/20240918/, and the\n  integrator-published setup reference https://documents.trocco.io/docs/connection-configuration-bakuraku\nnote: >-\n  Derived from provider terms plus published integrator setup docs. LayerX publishes no\n  OpenAPI, so there is no securitySchemes block to derive from; the API reference at\n  https://api.bakuraku.layerx.jp/rest/docs/ answers 401 WWW-Authenticate: Basic to\n  anonymous callers, so the header name and exact key format could not be verified and\n  are recorded as unknown rather than guessed.\napi: Bakuraku API\nbase_url: https://api.bakuraku.layerx.jp/rest\nschemes:\n- id: bakuraku-api-key\n  type: apiKey\n  name: unknown\n  in: unknown\n  label: Bakuraku API key\n  description: >-\n    A tenant-scoped API key issued from the Bakuraku\
  \ admin console. Per the integrator\n    setup reference the flow is: Bakuraku 管理画面 → API管理 → 新規作成 → select the\n    permissions the key should carry → issue the key. Article 4 of the API terms states\n    LayerX issues \"API認証情報\" to an approved \"API契約者\" and that the contract holder\n    bears full responsibility for its safekeeping; the credential may be shared with the\n    contract holder's own end users but never transferred, lent or sold to third parties.\n  issued_to: >-\n    An \"API契約者\" — a legal entity LayerX has approved for API use by its prescribed\n    application process. An existing Bakuraku subscription is a precondition (API terms,\n    Article 3).\n  header: unknown\n  rotation: >-\n    LayerX may suspend or re-issue API credentials without the contract holder's consent\n    while an incident is being contained (API terms, Article 6.5).\npermissions:\n  model: >-\n    Permission-scoped API keys. The permissions a key carries are selected at issuance in\n    the admin\
  \ console, so a key is least-privilege by construction rather than by an OAuth\n    scope string. This is not an OAuth 2.0 surface, so no scopes/ artifact is emitted.\n  observed:\n  - id: application-read\n    label: 申請の読み取り権限\n    english: Read applications / requests\n    source: https://documents.trocco.io/docs/connection-configuration-bakuraku\n  - id: org-chart-read\n    label: 組織図の読み取り権限\n    english: Read organization chart (groups and positions)\n    source: https://documents.trocco.io/docs/connection-configuration-bakuraku\n  - id: user-read\n    label: ユーザーの読み取り権限\n    english: Read users\n    source: https://documents.trocco.io/docs/connection-configuration-bakuraku\n  completeness: >-\n    Partial. These three are the permissions one named integrator documents needing for a\n    read-only sync. The full permission catalogue is inside the gated reference and has\n    not been observed.\noauth2:\n  present_on_api: false\n  note: >-\n    LayerX does operate an OAuth 2.0 / OIDC\
  \ authorization server for LayerX ID\n    (id.layerx.jp), built on Authlete and announced 2023-02-15. That server backs product\n    sign-in and SSO, not the Bakuraku REST API, and it publishes no anonymous\n    /.well-known/openid-configuration — every /.well-known/* path on id.layerx.jp returns\n    the sign-in SPA shell. Recorded here so a later round does not re-derive it as an\n    API auth flow.\n  source: https://www.authlete.com/ja/news-jp/20230215-layerx\ntenant_sso:\n  saml: true\n  note: >-\n    Bakuraku supports SAML single sign-on and IP address restrictions for tenant login\n    (customer-facing, not an API auth mode).\n  source: https://bakuraku.jp/security/\ntransport:\n  tls: true\n  observed_hsts: 'strict-transport-security: max-age=15552000; includeSubDomains'\n  observed_on: https://api.bakuraku.layerx.jp/rest/v1/tenant/users\n  probed: '2026-08-23'\ngaps:\n- No public OpenAPI or securitySchemes declaration.\n- Credential header name and key format not published anonymously.\n\
  - No published permission/scope reference page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/layerx/refs/heads/main/authentication/layerx-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Japan
- Back Office
- Expense Management
- Invoicing
- Accounts Payable
- Workflow
- Approvals
- Accounting
- Payroll
- Attendance
- Corporate Cards
- Artificial Intelligence
- AI Agents
- Document Processing
- SaaS
- Enterprise Software
- Fintech
---
