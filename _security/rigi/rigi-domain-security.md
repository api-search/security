---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rigi.club
  spf: true
hosts:
- cert_expires: Sep 26 12:47:24 2026 GMT
  host: app.rigi.club
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rigi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rigi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rigi
provider_slug: rigi
slug: rigi-domain-security
source_filename: rigi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app.rigi.club\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 12:47:24 2026 GMT\n  hsts: null\ndomains:\n- domain: rigi.club\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rigi/refs/heads/main/security/rigi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Media
- Entertainment
- Streaming
- Video
- Short-form Video
- OTT
- Mobile App
- India
---
