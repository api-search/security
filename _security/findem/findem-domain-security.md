---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: findem.ai
  spf: true
hosts:
- cert_expires: Aug 16 00:09:15 2026 GMT
  host: www.findem.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: app.findem.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Findem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Findem, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Findem
provider_slug: findem
slug: findem-domain-security
source_filename: findem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.findem.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 00:09:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.findem.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: findem.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/findem/refs/heads/main/security/findem-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Talent Intelligence
- AI Sourcing
- Talent Analytics
- Agentic AI
- Embedded AI
- HR Tech
---
