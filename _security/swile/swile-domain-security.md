---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: swile.co
  spf: true
hosts:
- cert_expires: Aug 20 11:51:47 2026 GMT
  host: www.swile.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Swile Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Swile, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Swile
provider_slug: swile
slug: swile-domain-security
source_filename: swile-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.swile.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 11:51:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: swile.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swile/refs/heads/main/security/swile-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Employee Benefits
- Meal Vouchers
- Payments
- Prepaid Cards
- Employee Engagement
- Human Resources
- Mastercard
---
