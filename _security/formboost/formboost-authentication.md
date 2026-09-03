---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Formboost Authentication
name_suffix: Authentication
oauth_flows: []
overview: Formboost declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Formboost
provider_slug: formboost
scheme_count: 4
schemes:
- description: No authentication. Anyone who knows a form's alias can post to it. This is the intended model for a form backend — the endpoint sits in public HTML where any visitor can read it.
  evidence: Live POST with no credentials on 2026-09-02 returned HTTP 202 {"success":true,"message":"Submission accepted for processing"}.
  id: none
  in: null
  method: probed
  surface: POST https://formboost.app/f/{alias}
  type: none
- bearer_format: JWT
  description: '"Dashboard access uses signed JWTs, and new accounts must verify their email address before the API accepts a request from them."'
  evidence: https://formboost.app/security
  id: dashboard-jwt
  method: searched
  public: false
  scheme: bearer
  surface: dashboard.formboost.app / service.formboost.app
  type: http
- description: Sign-in is backed by Google Firebase; account records store "a bcrypt-hashed password or a Firebase identity."
  evidence: https://formboost.app/security
  id: firebase-identity
  method: searched
  provider: Google Firebase
  public: false
  surface: dashboard.formboost.app
  type: openIdConnect
- description: The one native OAuth connection Formboost operates. It is an outbound authorization the customer grants to Formboost, not a way to authenticate INTO Formboost.
  evidence: https://formboost.app/llms.txt
  id: google-oauth-drive-file
  method: searched
  provider: Google
  scopes:
  - description: Per-file Drive access. Formboost states it requests ONLY drive.file, so it can reach the spreadsheets it created and nothing else in the user's Drive.
    name: https://www.googleapis.com/auth/drive.file
  surface: Google Sheets integration
  type: oauth2
slug: formboost-authentication
source_filename: formboost-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: >-\n  https://formboost.app/docs/api-reference-and-config, https://formboost.app/security,\n  https://formboost.app/llms.txt, plus live probes of https://formboost.app/f/{alias} 2026-09-02\nsummary: >-\n  The public Formboost surface is UNAUTHENTICATED by design. The only endpoint an external client\n  calls — POST https://formboost.app/f/{alias} — takes no key, no token and no header; the form\n  alias in the URL is the entire credential. Everything that requires an identity (creating\n  forms, reading submissions, configuring integrations) lives behind the dashboard, whose API is\n  not publicly documented and whose host answers 403 to anonymous requests.\nschemes:\n  - id: none\n    surface: POST https://formboost.app/f/{alias}\n    type: none\n    in: null\n    description: >-\n      No authentication. Anyone who knows a form's alias can post to it. This is the intended\n      model for a form backend — the endpoint sits\
  \ in public HTML where any visitor can read it.\n    method: probed\n    evidence: >-\n      Live POST with no credentials on 2026-09-02 returned HTTP 202\n      {\"success\":true,\"message\":\"Submission accepted for processing\"}.\n  - id: dashboard-jwt\n    surface: dashboard.formboost.app / service.formboost.app\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    description: >-\n      \"Dashboard access uses signed JWTs, and new accounts must verify their email address before\n      the API accepts a request from them.\"\n    public: false\n    method: searched\n    evidence: https://formboost.app/security\n  - id: firebase-identity\n    surface: dashboard.formboost.app\n    type: openIdConnect\n    provider: Google Firebase\n    description: >-\n      Sign-in is backed by Google Firebase; account records store \"a bcrypt-hashed password or a\n      Firebase identity.\"\n    public: false\n    method: searched\n    evidence: https://formboost.app/security\n  - id: google-oauth-drive-file\n\
  \    surface: Google Sheets integration\n    type: oauth2\n    provider: Google\n    scopes:\n      - name: https://www.googleapis.com/auth/drive.file\n        description: >-\n          Per-file Drive access. Formboost states it requests ONLY drive.file, so it can reach\n          the spreadsheets it created and nothing else in the user's Drive.\n    description: >-\n      The one native OAuth connection Formboost operates. It is an outbound authorization the\n      customer grants to Formboost, not a way to authenticate INTO Formboost.\n    method: searched\n    evidence: https://formboost.app/llms.txt\noutbound_auth:\n  description: >-\n    For webhook delivery the direction of trust reverses: the customer supplies custom headers\n    (Authorization, X-API-Key, anything) that Formboost attaches to each delivery so the\n    receiving endpoint can authenticate it.\n  docs: https://formboost.app/docs/http-webhook\n  inbound_verification: false\n  inbound_verification_note: >-\n    Formboost\
  \ does not sign deliveries. There is no HMAC header, so a consumer cannot verify\n    a payload came from Formboost. See asyncapi/formboost-webhooks.yml.\noauth_scopes_artifact: false\noauth_scopes_note: >-\n  No scopes/ artifact is written. The only OAuth in play is the outbound Google drive.file grant\n  recorded above; Formboost issues no tokens of its own and exposes no scope surface to consume.\nabuse_controls:\n  - control: per-IP rate limiting on the public endpoint\n    detail: 10 requests / 60s observed. See rate-limits/formboost-rate-limits.yml.\n    evidence: live probe 2026-09-02\n  - control: body size limit\n    detail: The public submission endpoint \"rejects oversized bodies.\"\n    evidence: https://formboost.app/security\n  - control: spam screening before storage\n    detail: Heuristics on every plan; Gemini AI screening from Starter up.\n    evidence: https://formboost.app/security\n  - control: allowed origins\n    detail: >-\n      Per-endpoint allowed-origin configuration\
  \ is offered in the dashboard, so a form alias can\n      be restricted to posting from the customer's own domains.\n    evidence: https://formboost.app/docs/api-reference-and-config\n  - control: non-enumerable aliases\n    detail: >-\n      A POST to a non-existent alias returns 202, not 404, so the endpoint does not confirm\n      whether an alias exists. Observed live 2026-09-02.\n    evidence: live probe 2026-09-02\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/formboost/refs/heads/main/authentication/formboost-authentication.yml
summary_line: 4 schemes
tags:
- forms
- form-backend
- html-forms
- serverless
- static-sites
- react
- nextjs
- vue
- webhooks
- no-code
- developer-tools
- spam-filtering
---
