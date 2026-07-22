---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: atombank.co.uk
  spf: true
hosts:
- cert_expires: Feb  7 14:00:25 2027 GMT
  host: www.atombank.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Atom Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atom Bank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Atom Bank
provider_slug: atom-bank
slug: atom-bank-domain-security
source_filename: atom-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.atombank.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 14:00:25 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: atombank.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atom-bank/refs/heads/main/security/atom-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Banking
- Digital Bank
- Challenger Bank
- Open Banking
- Mortgages
- Savings
- Lending
- United Kingdom
---
