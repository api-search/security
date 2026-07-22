---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tradewindmarkets.com
  spf: true
hosts:
- cert_expires: Sep 12 21:57:20 2026 GMT
  host: www.tradewindmarkets.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tradewind Markets Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tradewind Markets, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Tradewind Markets
provider_slug: tradewind-markets
slug: tradewind-markets-domain-security
source_filename: tradewind-markets-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tradewindmarkets.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 21:57:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: tradewindmarkets.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tradewind-markets/refs/heads/main/security/tradewind-markets-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Fintech
- Precious Metals
- Blockchain
- Commodities
- Gold
- Distributed Ledger
- Custody
---
