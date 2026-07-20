---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gamma.app
  spf: true
hosts:
- cert_expires: Oct  7 22:45:40 2026 GMT
  host: gamma.app
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 23:41:05 2026 GMT
  host: developers.gamma.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 22:45:40 2026 GMT
  host: public-api.gamma.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gamma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gamma, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gamma
provider_slug: gamma
slug: gamma-domain-security
source_filename: gamma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gamma.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 22:45:40 2026 GMT\n  hsts: null\n- host: developers.gamma.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:41:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: public-api.gamma.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 22:45:40 2026 GMT\n  hsts: null\ndomains:\n- domain: gamma.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gamma/refs/heads/main/security/gamma-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Productivity
- Presentations
- Documents
- Websites
- Artificial Intelligence
- Generative AI
- Content Generation
- Design
---
