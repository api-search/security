---
api_specs:
- filename: macroscope-webhook-api.json
  format: json
  label: Macroscope Agent Webhook API
  slug: macroscope-agent-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macroscope/refs/heads/main/openapi/macroscope-webhook-api.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: macroscope.com
  spf: true
hosts:
- cert_expires: Sep 22 11:32:04 2026 GMT
  host: docs.macroscope.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 10:59:34 2026 GMT
  host: hooks.macroscope.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Macroscope Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Macroscope, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Macroscope
provider_slug: macroscope
slug: macroscope-domain-security
source_filename: macroscope-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.macroscope.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 11:32:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: hooks.macroscope.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 10:59:34 2026 GMT\n  hsts: null\ndomains:\n- domain: macroscope.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/macroscope/refs/heads/main/security/macroscope-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Code Review
- Code Intelligence
- Developer Tools
- Pull Requests
- Agent
- Webhooks
- DevOps
---
