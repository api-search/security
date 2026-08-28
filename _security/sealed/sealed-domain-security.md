---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sealed.com
  spf: true
hosts:
- cert_expires: Oct  5 02:46:28 2026 GMT
  host: www.sealed.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sealed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sealed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sealed
provider_slug: sealed
slug: sealed-domain-security
source_filename: sealed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sealed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 02:46:28 2026 GMT\n  hsts: false\ndomains:\n- domain: sealed.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sealed/refs/heads/main/security/sealed-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Energy
- Energy Efficiency
- Climate Tech
- Home Services
- HVAC
- Electrification
- Rebates
- Incentives
- Contractors
- Utilities
- Weatherization
---
