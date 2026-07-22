---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lexspot.com
  spf: true
hosts:
- cert_expires: Sep 10 09:59:22 2026 GMT
  host: www.lexspot.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lexspot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LexSpot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: LexSpot
provider_slug: lexspot
slug: lexspot-domain-security
source_filename: lexspot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lexspot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 09:59:22 2026 GMT\n  hsts: null\ndomains:\n- domain: lexspot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lexspot/refs/heads/main/security/lexspot-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Stub
- Portfolio
- 500 Global
- Unverified
- Lead
---
