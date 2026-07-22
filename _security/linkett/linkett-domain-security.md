---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: linkett.com
  spf: true
hosts:
- cert_expires: Aug 23 19:42:24 2026 GMT
  host: linkett.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Linkett Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Linkett, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Linkett
provider_slug: linkett
slug: linkett-domain-security
source_filename: linkett-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: linkett.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 19:42:24 2026 GMT\n  hsts: false\ndomains:\n- domain: linkett.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linkett/refs/heads/main/security/linkett-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Advertising
- Digital Signage
- Digital Out Of Home
- DOOH
- Analytics
- Audience Measurement
- Retail Media
---
