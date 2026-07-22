---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: grove.co
  spf: true
hosts:
- cert_expires: Oct 12 06:20:13 2026 GMT
  host: grove.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Grove Collaborative Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Grove Collaborative, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Grove Collaborative
provider_slug: grove-collaborative
slug: grove-collaborative-domain-security
source_filename: grove-collaborative-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: grove.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 06:20:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: grove.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grove-collaborative/refs/heads/main/security/grove-collaborative-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer Products
- E-commerce
- Sustainability
- Household Products
- Personal Care
- Retail
---
