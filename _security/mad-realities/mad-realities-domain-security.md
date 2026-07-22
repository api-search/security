---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: madrealities.xyz
  spf: false
hosts:
- cert_expires: Jan 26 09:49:23 2027 GMT
  host: madrealities.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mad Realities Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mad Realities, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Mad Realities
provider_slug: mad-realities
slug: mad-realities-domain-security
source_filename: mad-realities-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: madrealities.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 09:49:23 2027 GMT\n  hsts: null\ndomains:\n- domain: madrealities.xyz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mad-realities/refs/heads/main/security/mad-realities-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Consumer
- Entertainment
- Media
- Creators
- Video
- Streaming
---
