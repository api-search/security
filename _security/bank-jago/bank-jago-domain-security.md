---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: jago.com
  spf: true
hosts:
- cert_expires: Oct  7 14:01:06 2026 GMT
  host: www.jago.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Bank Jago Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bank Jago, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Bank Jago
provider_slug: bank-jago
slug: bank-jago-domain-security
source_filename: bank-jago-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jago.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  7 14:01:06 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: jago.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bank-jago/refs/heads/main/security/bank-jago-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Banking
- Digital Bank
- Indonesia
- Open Banking
- Payments
- SNAP
---
