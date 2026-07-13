---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: onafriq.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mfsafrica.com
  spf: false
hosts:
- cert_expires: Sep  7 12:44:30 2026 GMT
  host: onafriq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 14:40:04 2026 GMT
  host: developers.onafriq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.mfsafrica.com
  https: false
kind: domain-security
layout: security
method: probed
name: Onafriq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Onafriq, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Onafriq
provider_slug: onafriq
slug: onafriq-domain-security
source_filename: onafriq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: onafriq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 12:44:30 2026 GMT\n  hsts: false\n- host: developers.onafriq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 14:40:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.mfsafrica.com\n  https: false\ndomains:\n- domain: onafriq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: mfsafrica.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onafriq/refs/heads/main/security/onafriq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Mobile Money
- Remittance
- Cross-Border Payments
- Disbursements
- Payouts
- Collections
- Bank Transfers
- Card Issuance
- Agent Banking
- Treasury
- Foreign Exchange
- Webhooks
- Africa
- Fintech
- Financial Services
- MFS Africa
- Onafriq
- Baxi
---
