---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: trybeem.com
  spf: true
hosts:
- cert_expires: Aug 20 18:47:11 2026 GMT
  host: trybeem.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beem, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Beem
provider_slug: beem
slug: beem-domain-security
source_filename: beem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trybeem.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 18:47:11 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: trybeem.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beem/refs/heads/main/security/beem-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Fintech
- Consumer Finance
- Cash Advance
- Personal Loans
- Banking
- Payments
- Mobile App
---
