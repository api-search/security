---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: trykarat.com
  spf: true
hosts:
- cert_expires: Sep 19 20:04:05 2026 GMT
  host: www.trykarat.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Karatio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Karat.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Karat.io
provider_slug: karatio
slug: karatio-domain-security
source_filename: karatio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trykarat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 20:04:05 2026 GMT\n  hsts: null\ndomains:\n- domain: trykarat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/karatio/refs/heads/main/security/karatio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Business Banking
- Payments
- Bookkeeping
- Creator Economy
- Small Business
---
