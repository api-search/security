---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: anna.money
  spf: true
hosts:
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: www.anna.money
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anna Money Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ANNA Money, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ANNA Money
provider_slug: anna-money
slug: anna-money-domain-security
source_filename: anna-money-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.anna.money\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: anna.money\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anna-money/refs/heads/main/security/anna-money-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial-Services
- Banking
- Fintech
- Business Account
- Open Banking
- PSD2
- Account Information
- Payments
- E-Money
- United Kingdom
- SME
---
