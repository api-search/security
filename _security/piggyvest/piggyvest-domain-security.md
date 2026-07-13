---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: piggyvest.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: piggyvestbusiness.com
  spf: false
hosts:
- cert_expires: Oct  2 05:20:04 2026 GMT
  host: www.piggyvest.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 23:30:37 2026 GMT
  host: www.piggyvestbusiness.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 17:32:50 2026 GMT
  host: api.piggyvest.business
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Piggyvest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PiggyVest, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: PiggyVest
provider_slug: piggyvest
slug: piggyvest-domain-security
source_filename: piggyvest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.piggyvest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 05:20:04 2026 GMT\n  hsts: false\n- host: www.piggyvestbusiness.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:30:37 2026 GMT\n  hsts: false\n- host: api.piggyvest.business\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 17:32:50 2026 GMT\n  hsts: null\ndomains:\n- domain: piggyvest.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: piggyvestbusiness.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/piggyvest/refs/heads/main/security/piggyvest-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Fintech
- Savings
- Investments
- Digital Wallet
- Micro Savings
- Goal Based Savings
- Fixed Deposit
- Dollar Savings
- Consumer Finance
- Personal Finance
- Mobile Banking
- Business Banking
- Wallet API
- Transfers
- Bank Transfers
- Scheduled Payments
- Webhooks
- Hosted Checkout
- Pay With Pocket
- Invoicing
- Reserved Accounts
- Africa
- Nigeria
- Lagos
---
