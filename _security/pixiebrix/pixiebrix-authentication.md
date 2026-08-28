---
api_key_in: []
api_specs:
- filename: pixiebrix-openapi.yml
  format: yaml
  label: PixieBrix Developer API
  slug: pixiebrix-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixiebrix/refs/heads/main/openapi/pixiebrix-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Pixiebrix Authentication
name_suffix: Authentication
oauth_flows: []
overview: PixieBrix declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: PixieBrix
provider_slug: pixiebrix
scheme_count: 1
schemes:
- applies_to: all operations except GET /api/health/
  description: Django-REST-Framework style token authentication. The value is the token issued when a Service Account is created in the PixieBrix Admin Console, prefixed with the literal word "Token" and a space.
  docs: https://docs.pixiebrix.com/developer-api/making-an-api-request
  format: Token <token>
  id: serviceAccountToken
  in: header
  name: Authorization
  required: true
  type: apiKey
slug: pixiebrix-authentication
source_filename: pixiebrix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://docs.pixiebrix.com/developer-api/making-an-api-request\ndocs: https://docs.pixiebrix.com/developer-api/making-an-api-request#authentication\nnote: >-\n  DERIVED FROM DOCS, NOT FROM THE SPEC. The published OpenAPI\n  (openapi/pixiebrix-openapi.yml) declares components.securitySchemes as EMPTY and\n  carries no top-level or per-operation `security` block, even though all 291\n  operations except GET /api/health/ require a token. This is a real, reportable\n  contract gap: a generated client or an agent reading only the spec cannot tell\n  the API is authenticated. The auth model below is taken verbatim from the\n  provider's own documentation.\nspec_declares_security: false\nschemes:\n  - id: serviceAccountToken\n    type: apiKey\n    in: header\n    name: Authorization\n    format: 'Token <token>'\n    description: >-\n      Django-REST-Framework style token authentication. The value is the token\n      issued when a\
  \ Service Account is created in the PixieBrix Admin Console,\n      prefixed with the literal word \"Token\" and a space.\n    docs: https://docs.pixiebrix.com/developer-api/making-an-api-request\n    required: true\n    applies_to: all operations except GET /api/health/\ncredential_issuance:\n  mechanism: Service Account\n  docs: https://docs.pixiebrix.com/developer-api/service-accounts\n  description: >-\n    Service Accounts are API-only users, permissioned like human team members but\n    excluded from subscription seat utilization. Created from the Admin Console\n    (\"Service Accounts\" > \"Create Service Account\"); the token is shown once in a\n    \"Service Account Created\" modal.\n  role_assignment: Role is chosen at creation time and CANNOT be changed afterwards.\n  rotation: not documented\n  expiry: not documented\n  availability:\n    - plan: Team\n      service_accounts: 1\n    - plan: Business\n      service_accounts: unlimited\n    - plan: Enterprise\n      service_accounts:\
  \ custom\noauth2: false\noauth2_note: >-\n  PixieBrix's own Developer API does not use OAuth 2.0 - it is token-only, so no\n  scopes/ artifact is emitted. PixieBrix does act as an OAuth 2.0 CLIENT for the\n  third-party services its bricks integrate with (documented at\n  https://docs.pixiebrix.com/integrations/oauth2-client-credentials), but that is a\n  consumer-side integration surface, not an authorization surface on this API.\nend_user_sso:\n  saml2: true\n  note: SAML 2.0 SSO and domain capture are available on the Enterprise plan for\n    Admin Console / extension sign-in, not for Developer API calls.\n  docs: https://docs.pixiebrix.com/enterprise-it-setup/authentication/setting-up-saml-sso\ncors:\n  supported: false\n  note: >-\n    \"The Developer API does not currently support Cross-Origin Resource Sharing\n    (CORS).\" Callers from a browser app must proxy through a backend.\n  source: https://docs.pixiebrix.com/developer-api/making-an-api-request\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pixiebrix/refs/heads/main/authentication/pixiebrix-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Browser Extensions
- Low-Code
- Automation
- Artificial Intelligence
- Customer Support
- Enterprise Operations
- Workflow Automation
- Agent Governance
- Robotic Process Automation
---
