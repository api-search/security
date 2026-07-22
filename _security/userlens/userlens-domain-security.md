---
api_specs:
- filename: userlens-events-openapi.yml
  format: yaml
  label: Userlens Events API
  slug: userlens-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/userlens/refs/heads/main/openapi/userlens-events-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: userlens.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gitbook.io
  spf: true
hosts:
- cert_expires: Oct  6 18:53:48 2026 GMT
  host: userlens.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 19:03:12 2026 GMT
  host: userlens.gitbook.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 08:29:27 2026 GMT
  host: events.userlens.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Userlens Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Userlens, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Userlens
provider_slug: userlens
slug: userlens-domain-security
source_filename: userlens-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: userlens.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 18:53:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: userlens.gitbook.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 19:03:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: events.userlens.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 08:29:27 2026 GMT\n  hsts: null\ndomains:\n- domain: userlens.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: gitbook.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/userlens/refs/heads/main/security/userlens-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Customer Success
- Product Analytics
- AI Agents
- Churn Prediction
- Event Tracking
- B2B SaaS
- Account Intelligence
---
