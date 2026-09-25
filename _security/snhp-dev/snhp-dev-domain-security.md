---
api_specs:
- filename: snhp-dev-openapi.yml
  format: yaml
  label: SNHP Game Theory Layer API
  slug: game-theory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snhp-dev/refs/heads/main/openapi/snhp-dev-openapi.yml
- filename: snhp-dev-arena-openapi.yml
  format: yaml
  label: SNHP Evolution Arena API
  slug: evolution-arena-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snhp-dev/refs/heads/main/openapi/snhp-dev-arena-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: snhp.dev
  spf: false
hosts:
- cert_expires: Nov 27 12:01:56 2026 GMT
  host: snhp.dev
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_note: 'strict-transport-security: max-age=31536000; includeSubDomains observed on every GET/POST response from snhp.dev on 2026-09-19 (the scripts HEAD did not record it)'
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  6 11:42:27 2026 GMT
  host: arena.snhp.dev
  hsts: false
  hsts_note: no strict-transport-security header observed on arena.snhp.dev responses
  https: true
  tls_version: TLSv1.3
- host: api.snhp.dev
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Alias of the same Fly.io application as snhp.dev; TLS 1.3 + HSTS observed on live responses 2026-09-19 (added from the curl observations, not the script)
  tls_version: TLSv1.3
- host: www.snhp.dev
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Alias of the same Fly.io application as snhp.dev; TLS 1.3 + HSTS observed on live responses 2026-09-19 (added from the curl observations, not the script)
  tls_version: TLSv1.3
- host: snhp.fly.dev
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Alias of the same Fly.io application as snhp.dev; TLS 1.3 + HSTS observed on live responses 2026-09-19 (added from the curl observations, not the script)
  tls_version: TLSv1.3
hosts_probed: 5
kind: domain-security
layout: security
method: probed
name: Snhp Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SNHP, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: SNHP
provider_slug: snhp-dev
slug: snhp-dev-domain-security
source_filename: snhp-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: snhp.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 12:01:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_note: 'strict-transport-security: max-age=31536000; includeSubDomains observed on every GET/POST response\n    from snhp.dev on 2026-09-19 (the scripts HEAD did not record it)'\n- host: arena.snhp.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 11:42:27 2026 GMT\n  hsts: false\n  hsts_note: no strict-transport-security header observed on arena.snhp.dev responses\n- host: api.snhp.dev\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: Alias of the same Fly.io application as snhp.dev; TLS 1.3 + HSTS observed on live responses 2026-09-19 (added\n    from the curl observations, not the script)\n- host: www.snhp.dev\n\
  \  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: Alias of the same Fly.io application as snhp.dev; TLS 1.3 + HSTS observed on live responses 2026-09-19 (added\n    from the curl observations, not the script)\n- host: snhp.fly.dev\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: Alias of the same Fly.io application as snhp.dev; TLS 1.3 + HSTS observed on live responses 2026-09-19 (added\n    from the curl observations, not the script)\ndomains:\n- domain: snhp.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\nsecurity_headers_observed:\n  host: snhp.dev\n  headers:\n  - 'strict-transport-security: max-age=31536000; includeSubDomains'\n  - 'x-content-type-options: nosniff'\n  - 'x-frame-options: DENY'\n  - 'referrer-policy: no-referrer'\n  - 'content-security-policy: default-src ''none''; frame-ancestors ''none''  (API responses); default-src\
  \ ''self''\n    ... (HTML pages)'\nemail_note: No SPF and no DMARC on snhp.dev; the operator contact is a gmail.com address, so no mail is expected\n  to originate from the domain — but nothing prevents spoofing it either.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snhp-dev/refs/heads/main/security/snhp-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Negotiation
- Game Theory
- AI Agents
- MCP
- A2A
- Agentic Payments
- Auctions
- Mechanism Design
- Pricing Optimization
- Artificial Intelligence
- Agent-Native
- Developer Tools
---
