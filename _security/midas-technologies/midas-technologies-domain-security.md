---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: midascash.app
  spf: true
hosts:
- cert_expires: Sep 30 00:12:04 2026 GMT
  host: midascash.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Midas Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MIDAS Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: MIDAS Technologies
provider_slug: midas-technologies
slug: midas-technologies-domain-security
source_filename: midas-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: midascash.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 00:12:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: midascash.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/midas-technologies/refs/heads/main/security/midas-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Fintech
- Payments
- Loyalty
- Rewards
- Consumer
- Mobile App
- Cashback
- Mexico
- Financial Inclusion
---
