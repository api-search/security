---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Qname Authentication
name_suffix: Authentication
oauth_flows: []
overview: QName AI WHOIS API declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: QName AI WHOIS API
provider_slug: qname
scheme_count: 0
schemes: []
slug: qname-authentication
source_filename: qname-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: searched\nsource: >-\n  @qname/cli source (bin/qname-cli.mjs, README.md), the published Agent Skill,\n  and https://qname.ai/cli. No OpenAPI securitySchemes exist (no published spec);\n  the auth profile is read from the official first-party client and docs.\napi: QName AI WHOIS REST API\nsummary: >-\n  Single-scheme API-key authentication. Every request carries an admin-approved\n  API key in the x-api-key HTTP header. Access is request-and-approve: a user\n  requests a key at /settings/apikeys, selects the API types (scopes) and quota\n  tiers they need, and an administrator approves it before it works.\nsecurity_schemes:\n  - type: apiKey\n    name: x-api-key\n    in: header\n    key_prefix: qname_\n    description: >-\n      Approved API key issued from QName.AI account settings. Sent as the\n      x-api-key request header on every call.\n    request_url: https://qname.ai/settings/apikeys\n    approval: admin-approved\n    gated: true\n\
  scopes:\n  - id: domain.query.whois.single\n    description: Single-domain WHOIS/RDAP lookup (GET /api/whois/{domain}).\n  - id: domain.query.whois.batch\n    description: Batch WHOIS/RDAP lookup (POST /api/whois/batch).\n  - id: domain.traffic.lookup\n    description: Domain traffic evidence (GET /api/domain-traffic).\nnotes: >-\n  Scopes above are QName \"API types\" attached to a key at approval time, not OAuth\n  scopes — there is no OAuth/OIDC flow. Keys are also constrained by a per-request\n  domain quota and a daily request quota chosen at approval. An unauthenticated or\n  bot request to the API host returns 403 (Cloudflare Turnstile: TURNSTILE_REQUIRED);\n  a bad key returns 401.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qname/refs/heads/main/authentication/qname-authentication.yml
summary_line: 0 schemes
tags:
- WHOIS
- RDAP
- domain-research
- Domain Search
- batch-lookup
- CLI
- Agent Tooling
- Agent Skills
- llms-txt
- Developer Tools
- Domain Intelligence
---
