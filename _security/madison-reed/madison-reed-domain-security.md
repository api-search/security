---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: madison-reed.com
  spf: true
hosts:
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: madison-reed.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Madison Reed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Madison-reed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Madison-reed
provider_slug: madison-reed
slug: madison-reed-domain-security
source_filename: madison-reed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: madison-reed.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: madison-reed.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/madison-reed/refs/heads/main/security/madison-reed-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Beauty
- Hair Color
- Cosmetics
- Direct to Consumer
- E-Commerce
- Retail
- Consumer Goods
---
