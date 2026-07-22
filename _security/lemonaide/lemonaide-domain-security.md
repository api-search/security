---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: lemonaide.co.th
  spf: true
hosts:
- cert_expires: Sep 11 13:28:55 2026 GMT
  host: lemonaide.co.th
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lemonaide Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lemonaide, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Lemonaide
provider_slug: lemonaide
slug: lemonaide-domain-security
source_filename: lemonaide-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lemonaide.co.th\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 13:28:55 2026 GMT\n  hsts: false\ndomains:\n- domain: lemonaide.co.th\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lemonaide/refs/heads/main/security/lemonaide-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Automotive
- Used Cars
- Insurance
- Insurtech
- Dealer Management
- SaaS
- Southeast Asia
- Thailand
- Escrow
---
