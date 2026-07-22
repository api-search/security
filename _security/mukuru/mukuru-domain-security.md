---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mukuru.com
  spf: true
hosts:
- cert_expires: Aug 26 10:48:32 2026 GMT
  host: www.mukuru.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mukuru Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mukuru, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mukuru
provider_slug: mukuru
slug: mukuru-domain-security
source_filename: mukuru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mukuru.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 10:48:32 2026 GMT\n  hsts: null\ndomains:\n- domain: mukuru.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mukuru/refs/heads/main/security/mukuru-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Remittance
- Money Transfer
- Cross Border Payments
- Africa
- South Africa
- Diaspora
- Mobile Money
- Wallet
- Prepaid Card
- Funeral Insurance
- Disbursements
- Collections
- Cash In Cash Out
- Financial Inclusion
- Fintech
---
