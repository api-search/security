---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: breef.com
  spf: true
hosts:
- cert_expires: Oct  1 05:46:58 2026 GMT
  host: www.breef.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Breef Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Breef, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Breef
provider_slug: breef
slug: breef-domain-security
source_filename: breef-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.breef.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 05:46:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: breef.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/breef/refs/heads/main/security/breef-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketing
- Advertising
- Agencies
- Marketplace
- Creative Services
- Procurement
- Payments
- Software-as-a-Service
---
