---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: depay.us
  spf: true
hosts:
- cert_expires: Sep  7 04:36:58 2026 GMT
  host: depay.us
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Depay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Depay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Depay
provider_slug: depay
slug: depay-domain-security
source_filename: depay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: depay.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 04:36:58 2026 GMT\n  hsts: false\ndomains:\n- domain: depay.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/depay/refs/heads/main/security/depay-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Payments
- Cross-Border Payments
- Fintech
- Instant Payments
- Latin America
- QR Payments
- Payment Infrastructure
---
