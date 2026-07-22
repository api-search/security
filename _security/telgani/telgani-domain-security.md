---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: telgani.com
  spf: true
hosts:
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: telgani.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Telgani Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Telgani, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Telgani
provider_slug: telgani
slug: telgani-domain-security
source_filename: telgani-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: telgani.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: telgani.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telgani/refs/heads/main/security/telgani-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Car Rental
- Mobility
- Marketplace
- Travel
- Transportation
- Saudi Arabia
- Consumer App
---
