---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: snapette.com
  spf: false
hosts:
- cert_expires: Sep  7 03:59:30 2026 GMT
  host: snapette.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Snapette Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Snapette, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Snapette
provider_slug: snapette
slug: snapette-domain-security
source_filename: snapette-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: snapette.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 03:59:30 2026 GMT\n  hsts: false\ndomains:\n- domain: snapette.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snapette/refs/heads/main/security/snapette-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Fashion
- E-Commerce
- Mobile
- Shopping
- Defunct
---
