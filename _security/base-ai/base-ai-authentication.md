---
api_key_in:
- unknown
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Base Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Base Ai secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Base Ai
provider_slug: base-ai
scheme_count: 1
schemes:
- description: Base account API token. Generated inside the logged-in Base application at Settings → "Users & Team" → "Generate token", supplying a Name and a Comment. The token is shown once and must be stored by the customer. Token issuance therefore requires an existing Base account — the API is customer-only, not open to public sign-up.
  in: unknown
  issuance:
    fields:
    - Name
    - Comment
    location: Base web application (https://go.base.ai)
    path: Settings > Users & Team > Generate token
    requires_account: true
    self_service: true
  name: apiToken
  sources:
  - https://www.unifyapps.com/docs/unify-integrations/base-ai
  type: apiKey
slug: base-ai-authentication
source_filename: base-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://www.unifyapps.com/docs/unify-integrations/base-ai\nfirst_party_documentation: false\nfirst_party_docs_note: >-\n  Base publishes NO public API reference, developer portal or authentication page. api.base.ai,\n  developer.base.ai, docs.base.ai and app.base.ai do not resolve; www.base.ai returns 404 for\n  /openapi.json, /swagger.json, /api-docs, /docs and /graphql. The auth model below is recorded\n  from a third-party integration platform's connector documentation, which quotes Base's own\n  in-product token screen verbatim. It is real and citable, but it is not published by Base.\nsummary:\n  types: [apiKey]\n  api_key_in: [unknown]\n  oauth2_flows: []\n  note: >-\n    Header/parameter placement of the token is not stated by any public source and was not\n    observable without an account, so api_key_in is recorded as unknown rather than guessed.\nschemes:\n- name: apiToken\n  type: apiKey\n  in: unknown\n  description:\
  \ >-\n    Base account API token. Generated inside the logged-in Base application at\n    Settings → \"Users & Team\" → \"Generate token\", supplying a Name and a Comment. The token is\n    shown once and must be stored by the customer. Token issuance therefore requires an existing\n    Base account — the API is customer-only, not open to public sign-up.\n  issuance:\n    location: Base web application (https://go.base.ai)\n    path: Settings > Users & Team > Generate token\n    fields: [Name, Comment]\n    self_service: true\n    requires_account: true\n  sources: ['https://www.unifyapps.com/docs/unify-integrations/base-ai']\nbase_url:\n  value: null\n  note: >-\n    No public source names an API host. The go.base.ai single-page app calls same-origin /api/*\n    routes (/api/authenticate, /api/authenticate/token, /api/authorization/privilege,\n    /api/integration, /api/project/version were read from its published JS bundle\n    /assets/index-B1hfJk0m.js), but the edge answers every unauthenticated\
  \ GET on go.base.ai with\n    the SPA HTML shell under HTTP 200, so the API host could not be confirmed by probe. Recorded\n    as missing rather than guessed.\nx-api-surface:\n  status: partner-documented\n  note: >-\n    NOT a Base-published contract and NOT an OpenAPI. This is the capability surface a third-party\n    iPaaS vendor exposes for its Base AI connector, which is evidence that a real token-authenticated\n    API exists and roughly what it covers. No request/response schemas, paths, methods or parameter\n    names are published anywhere public, so none are recorded here.\n  source: https://www.unifyapps.com/docs/unify-integrations/base-ai\n  source_last_updated: '2026-08-04'\n  action_count: 26\n  trigger_count: 4\n  domains: [users, advocates, accounts, opportunities, contacts, custom-attributes, reference-requests, points]\n  actions:\n  - Create a user\n  - Delete a user by email\n  - Delete user by ID\n  - List users\n  - List accounts\n  - List advocates\n  - List opportunities\n\
  \  - Upsert opportunity\n  - Update account custom attribute\n  - Update advocate custom attributes\n  - Create advocate custom object attributes\n  - Update advocate custom object attributes\n  - Delete advocate custom object attributes\n  - List custom attributes\n  - List custom object attributes\n  - Import contacts by contact ID\n  - Import contacts by email\n  - Grant points to advocate by API\n  - Trigger user's activity\n  - Notify when advocate completes an ASK\n  - Read reference request form settings\n  - Read submitted reference requests\n  - Read submitted reference requests by UUID\n  - Read the reference advocates\n  - Submit a reference request in managed or p2p mode\n  triggers:\n  - New advocate\n  - New or updated account\n  - New or updated opportunity\n  - New user\n  triggers_note: >-\n    These are the integration vendor's trigger names. Nothing public states whether Base delivers\n    them as webhooks or whether the vendor polls, so no Webhooks pointer is emitted.\n\
  x-evidence:\n- {url: 'https://www.unifyapps.com/docs/unify-integrations/base-ai', http_status: 200}\n- {url: 'https://www.base.ai/openapi.json', http_status: 404}\n- {url: 'https://www.base.ai/swagger.json', http_status: 404}\n- {url: 'https://www.base.ai/api-docs', http_status: 404}\n- {url: 'https://www.base.ai/graphql', http_status: 404}\n- {url: 'https://go.base.ai/openapi.json', http_status: 200, note: text/html SPA shell, not a spec}\n- {url: 'https://go.base.ai/assets/index-B1hfJk0m.js', http_status: 200, note: app bundle naming same-origin /api/* routes}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/base-ai/refs/heads/main/authentication/base-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- Customer-Led Growth
- Customer Success
- Customer Marketing
- Advocacy
- RevOps
- SaaS
---
