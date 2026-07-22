---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kuda.com
  spf: true
hosts:
- cert_expires: Sep 26 19:34:56 2026 GMT
  host: kuda.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Kuda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kuda, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kuda
provider_slug: kuda
slug: kuda-domain-security
source_filename: kuda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kuda.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 26 19:34:56 2026 GMT\n  hsts: false\ndomains:\n- domain: kuda.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kuda/refs/heads/main/security/kuda-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Banking
- Neobank
- Digital Bank
- Retail Banking
- Business Banking
- Open Banking
- Payments
- Transfers
- Virtual Accounts
- Disbursements
- Bill Payments
- Savings
- Cards
- POS
- Lending
- Fintech
- Nigeria
- Africa
- CBN Licensed
- Microfinance Bank
---
