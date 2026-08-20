---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: 17Hats Authentication
name_suffix: Authentication
oauth_flows: []
overview: 17hats declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: 17hats
provider_slug: 17hats
scheme_count: 1
schemes:
- applies_to: the contact operations exposed through the Zapier connector
  description: Static, account-scoped API key. Presented by the Zapier connector when linking a 17hats account. 17hats publishes the key's existence and where to obtain it, but not where it is placed on the wire — no public docs state a header name, query parameter, or base URL. Recorded as in/name unknown rather than assumed.
  id: account-api-key
  in: unknown
  issued_from: 17hats web app > Account Settings > Integrations > Zapier > Enable
  name: unknown
  required: true
  scope: whole account (no per-scope or per-resource restriction documented)
  type: apiKey
slug: 17hats-authentication
source_filename: 17hats-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://help.17hats.com/en/articles/2761371-zapier-integration\ndocs: https://help.17hats.com/en/articles/2761371-zapier-integration\napi: 17hats partner integration API (no public reference published)\nsummary: >-\n  17hats does not publish a public developer program, API reference or\n  machine-readable specification. The only programmatic credential 17hats\n  documents to its customers is an account-level API key, generated from\n  Account Settings > Integrations by enabling the Zapier section and copying the\n  key shown in the dialog. That key authenticates the 17hats Zapier app, whose\n  published surface is limited to contacts (triggers: New Contact, Updated\n  Contact; actions: Create Contact, Update Contact, Search Contact, Find or\n  Create Contact). 17hats does not document the request host, the header or\n  query parameter the key is presented in, an OAuth 2.0 or OpenID Connect flow,\n  scopes, token lifetimes,\
  \ or key rotation. The transport-level details are\n  therefore UNKNOWN and are deliberately left unrecorded rather than guessed.\nschemes:\n- id: account-api-key\n  type: apiKey\n  in: unknown\n  name: unknown\n  required: true\n  issued_from: 17hats web app > Account Settings > Integrations > Zapier > Enable\n  description: >-\n    Static, account-scoped API key. Presented by the Zapier connector when\n    linking a 17hats account. 17hats publishes the key's existence and where to\n    obtain it, but not where it is placed on the wire — no public docs state a\n    header name, query parameter, or base URL. Recorded as in/name unknown\n    rather than assumed.\n  applies_to: the contact operations exposed through the Zapier connector\n  scope: whole account (no per-scope or per-resource restriction documented)\noauth2: false\nopenid_connect: false\nscopes_documented: false\nplan_gating:\n  note: >-\n    17hats documents the Zapier integration as available only on its newer\n    subscription\
  \ plan, so the API key is plan-gated as well as account-gated.\n  source: https://help.17hats.com/en/articles/2761371-zapier-integration\nnotes:\n- No public API reference, developer portal, or OpenAPI/Swagger/GraphQL/AsyncAPI\n  document exists for 17hats. Contract discovery (STEP 0b) probed the API host\n  root, docs host, GraphQL introspection, MCP tools/list and both A2A well-known\n  paths; all missed. See well-known/17hats-well-known.yml.\n- api.17hats.com and developer.17hats.com resolve only because *.17hats.com is a\n  wildcard catch-all; neither is a real API host. Do not treat either as a\n  baseURL.\n- The only machine-consumable description of the 17hats surface a third party can\n  read today is the Zapier app listing at\n  https://zapier.com/apps/17hats/integrations, which is Zapier's document, not\n  17hats'.\nx-evidence:\n- url: https://help.17hats.com/en/articles/2761371-zapier-integration\n  http_status: 200\n  fetched: '2026-08-05'\n  finding: API key location + contacts-only\
  \ scope\n- url: https://zapier.com/apps/17hats/integrations\n  http_status: 200\n  fetched: '2026-08-05'\n  finding: 2 triggers + 4 actions, all Contacts\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/17hats/refs/heads/main/authentication/17hats-authentication.yml
summary_line: 1 scheme
tags:
- Company
- CRM
- Small Business
- Invoicing
- Scheduling
- Bookkeeping
- Workflow-Automation
- Contract Management
- Payments
- Software-as-a-Service
---
