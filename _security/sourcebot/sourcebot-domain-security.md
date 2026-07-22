---
api_specs:
- filename: sourcebot-public-openapi-original.json
  format: json
  label: Sourcebot Public API
  slug: sourcebot-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sourcebot/refs/heads/main/openapi/sourcebot-public-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sourcebot.dev
  spf: true
hosts:
- cert_expires: Sep 28 03:38:25 2026 GMT
  host: www.sourcebot.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 18:45:47 2026 GMT
  host: docs.sourcebot.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: app.sourcebot.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sourcebot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sourcebot, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sourcebot
provider_slug: sourcebot
slug: sourcebot-domain-security
source_filename: sourcebot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sourcebot.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 03:38:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.sourcebot.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 18:45:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.sourcebot.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sourcebot.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sourcebot/refs/heads/main/security/sourcebot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Code Search
- Code Intelligence
- Developer Tools
- Source Code
- Git
- MCP
- AI Coding Agents
- Enterprise Search
- Self-Hosted
---
