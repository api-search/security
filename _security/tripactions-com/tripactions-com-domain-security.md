---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tripactions.com
  spf: true
hosts:
- cert_expires: Dec 16 16:32:14 2026 GMT
  host: tripactions.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tripactions Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Navan, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Navan
provider_slug: tripactions-com
slug: tripactions-com-domain-security
source_filename: tripactions-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tripactions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 16:32:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tripactions.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/tripactions-com/security/tripactions-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Travel
- Expense Management
- SaaS
- Corporate
---
