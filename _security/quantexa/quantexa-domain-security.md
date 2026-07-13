---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: quantexa.com
  spf: true
hosts:
- cert_expires: Aug 12 21:53:51 2026 GMT
  host: www.quantexa.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quantexa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quantexa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Quantexa
provider_slug: quantexa
slug: quantexa-domain-security
source_filename: quantexa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.quantexa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 21:53:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: quantexa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quantexa/refs/heads/main/security/quantexa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Analytics
- Decision Intelligence
- Entity Resolution
- Graph Analytics
- Financial Crime
- Risk
- Customer Intelligence
- AI
---
