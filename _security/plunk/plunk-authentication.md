---
api_key_in:
- header
api_specs:
- filename: plunk-api-openapi.json
  format: json
  label: Plunk API
  slug: plunk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plunk/refs/heads/main/openapi/_original/plunk-api-openapi.json
- filename: plunk-campaigns-api-openapi.yml
  format: yaml
  label: Plunk Campaigns API
  slug: plunk-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plunk/refs/heads/main/openapi/plunk-campaigns-api-openapi.yml
- filename: plunk-contacts-api-openapi.yml
  format: yaml
  label: Plunk Contacts API
  slug: plunk-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plunk/refs/heads/main/openapi/plunk-contacts-api-openapi.yml
- filename: plunk-events-api-openapi.yml
  format: yaml
  label: Plunk Events API
  slug: plunk-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plunk/refs/heads/main/openapi/plunk-events-api-openapi.yml
- filename: plunk-transactional-api-openapi.yml
  format: yaml
  label: Plunk Transactional API
  slug: plunk-transactional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plunk/refs/heads/main/openapi/plunk-transactional-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Plunk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Plunk secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Plunk
provider_slug: plunk
scheme_count: 1
schemes:
- applied: global
  applied_note: The spec declares security ApiKeyAuth at the document root, applying to every operation.
  bearerFormat: API Key
  description: API key authentication. The project is derived automatically from the key, so no project identifier appears on any request. /v1/track requires a public key (pk_*) and rejects a secret key with 401; every other endpoint requires a secret key (sk_*) and rejects a public key with 401. The two key types are not interchangeable in either direction.
  format: Bearer <key>
  header: Authorization
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/_original/plunk-api-openapi.json
  type: http
slug: plunk-authentication
source_filename: plunk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/_original/plunk-api-openapi.json\ndocs: https://docs.useplunk.com/guides/api-keys\nsupersedes: >-\n  The 2026-07-11 derived pass, which read the hand-authored spec and reported a\n  single unqualified `bearerAuth` scheme. Plunk's published OpenAPI and its API\n  keys guide document a two-key model where the key PREFIX determines which\n  endpoints a credential may call — that split is the whole auth model and was\n  invisible in the derived file.\nsummary:\n  types: [http]\n  schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: []\n  key_classes: 2\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  header: Authorization\n  format: \"Bearer <key>\"\n  description: >-\n    API key authentication. The project is derived automatically from the key,\n    so no project identifier appears on any request. /v1/track requires a public\n    key (pk_*) and rejects a secret key with 401;\
  \ every other endpoint requires a\n    secret key (sk_*) and rejects a public key with 401. The two key types are\n    not interchangeable in either direction.\n  sources:\n  - openapi/_original/plunk-api-openapi.json\n  applied: global\n  applied_note: The spec declares security ApiKeyAuth at the document root, applying to every operation.\nkey_classes:\n- class: secret\n  prefix: 'sk_'\n  scope: >-\n    Every endpoint except POST /v1/track — sending email, contacts, segments,\n    campaigns, templates, workflows, domains, billing.\n  placement: server-side only\n  guidance: >-\n    Store in environment variables or the platform secret store. Never bundle\n    into a frontend build.\n- class: public\n  prefix: 'pk_'\n  scope: POST /v1/track only\n  placement: browser and mobile client code\n  guidance: >-\n    Deliberately limited so events can be recorded from a client without\n    exposing the project's full API surface. Treat as semi-sensitive and rotate\n    if the tracking endpoint\
  \ is being abused.\nmismatch_behavior:\n  status: 401\n  code: INVALID_API_KEY\n  message_example: 'Invalid secret API key. This endpoint requires a secret key (sk_*), not a public key.'\nmissing_credential:\n  status: 401\n  code: MISSING_AUTH\nrotation:\n  endpoint: \"POST /users/@me/projects/{id}/regenerate-keys\"\n  console: Settings -> API Keys\n  granularity: pair\n  granularity_note: >-\n    The two keys rotate together. There is no way to rotate one without\n    invalidating the other, and there is no grace period — the old keys stop\n    working immediately, so every consumer must be updated in one window.\n  recommended_triggers: [key committed to a public repository, offboarding a contractor, revoking a deployment, periodic rotation policy]\ncompromise_playbook:\n  source: https://docs.useplunk.com/guides/api-keys\n  steps:\n  - Rotate immediately.\n  - Audit the Activity tab for unexpected sends, contact mutations or campaign changes during the exposure window.\n  - Check Billing\
  \ -> Consumption for usage spikes.\n  - Report unauthorized activity to support with the request IDs from the suspicious entries.\nenvironment_separation:\n  test_mode: false\n  note: >-\n    There is NO test/live key split. pk_/sk_ is a capability split, not an\n    environment split, and Plunk publishes no sandbox or test-mode credentials.\n    The documented practice is to run separate Plunk PROJECTS for staging and\n    production so a leaked staging key cannot touch production data. This is why\n    no sandbox/ artifact exists in this repo.\noauth:\n  api_oauth: false\n  console_oauth: true\n  console_providers: [github, google]\n  console_note: >-\n    GET /auth/oauth-config reports which OAuth providers are configured, and\n    https://next-api.useplunk.com/config confirms github and google are enabled\n    on the hosted service. This is human sign-in to the dashboard, not API\n    authorization — there is no authorization server, no scopes and no token\n    endpoint, which is why\
  \ scopes/ is deliberately absent.\nself_hosting:\n  note: >-\n    Self-hosted deployments issue their own key pairs per project against their\n    own base URL; the model is identical because it is the same AGPL-3.0\n    codebase.\n  docs: https://docs.useplunk.com/self-hosting/introduction\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plunk/refs/heads/main/authentication/plunk-authentication.yml
summary_line: http · 1 scheme
tags:
- Email
- Transactional Email
- Marketing
- Automation
- Open-Source
- Software-as-a-Service
- Email API
- Webhook
- Segmentation
- Workflow-Automation
- Self-Hosted
- Developer Tools
---
