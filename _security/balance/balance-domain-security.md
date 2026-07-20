---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getbalance.com
  spf: true
hosts:
- cert_expires: Sep  7 10:31:33 2026 GMT
  host: getbalance.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Balance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Balance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Balance
provider_slug: balance
slug: balance-domain-security
source_filename: balance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getbalance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 10:31:33 2026 GMT\n  hsts: false\ndomains:\n- domain: getbalance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/balance/refs/heads/main/security/balance-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Payments
- B2B Payments
- Accounts Receivable
- Net Terms
- Trade Credit
- BNPL
- Billing
- Embedded Finance
---
