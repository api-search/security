---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cariqpay.com
  spf: true
hosts:
- cert_expires: Dec 13 07:15:20 2026 GMT
  host: www.cariqpay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Car Iq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Car IQ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Car IQ
provider_slug: car-iq
slug: car-iq-domain-security
source_filename: car-iq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cariqpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 07:15:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cariqpay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/car-iq/refs/heads/main/security/car-iq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Fleet Management
- FinTech
- API
---
