---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: acerta.ai
  spf: true
hosts:
- cert_expires: Aug 27 14:15:36 2026 GMT
  host: acerta.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Acerta Analytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acerta Analytics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Acerta Analytics
provider_slug: acerta-analytics
slug: acerta-analytics-domain-security
source_filename: acerta-analytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: acerta.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 14:15:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: acerta.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acerta-analytics/refs/heads/main/security/acerta-analytics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Manufacturing Analytics
- Industrial AI
- Machine Learning
- Quality
- Automotive
- Manufacturing
- Analytics
---
