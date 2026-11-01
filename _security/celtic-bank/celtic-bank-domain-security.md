---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: celticbank.com
  spf: true
hosts:
- cert_expires: Dec 16 03:44:14 2026 GMT
  host: celticbank.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Celtic Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Celtic Bank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Celtic Bank
provider_slug: celtic-bank
slug: celtic-bank-domain-security
source_filename: celtic-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: celticbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 03:44:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: celticbank.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/celtic-bank/security/celtic-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Finance
- SBA Loans
- Commercial Lending
- Fintech
---
