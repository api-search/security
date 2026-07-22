---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: storicard.com
  spf: true
hosts:
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: www.storicard.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stori Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stori, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Stori
provider_slug: stori
slug: stori-domain-security
source_filename: stori-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.storicard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: storicard.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stori/refs/heads/main/security/stori-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Financial Services
- Neobank
- Digital Bank
- Consumer Finance
- Credit Cards
- Financial Inclusion
- Underbanked
- Personal Loans
- Deposit Accounts
- Savings
- Bill Pay
- Mobile Banking
- Fintech
- Latin America
- Mexico
---
