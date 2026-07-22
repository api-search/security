---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kredete.io
  spf: true
hosts:
- cert_expires: Oct 15 07:37:20 2026 GMT
  host: www.kredete.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kredete Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kredete, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kredete
provider_slug: kredete
slug: kredete-domain-security
source_filename: kredete-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kredete.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 07:37:20 2026 GMT\n  hsts: false\ndomains:\n- domain: kredete.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kredete/refs/heads/main/security/kredete-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Financial Services
- Payments
- Remittance
- Cross-Border Payments
- Banking
- Credit
- Cards
- Savings
- Fintech
- Emerging Markets
- Africa
---
