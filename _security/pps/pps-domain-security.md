---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pps.tv
  spf: true
hosts:
- cert_expires: Aug 12 02:41:01 2026 GMT
  host: pps.tv
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PPS (pps.tv), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: PPS (pps.tv)
provider_slug: pps
slug: pps-domain-security
source_filename: pps-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pps.tv\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 02:41:01 2026 GMT\n  hsts: false\ndomains:\n- domain: pps.tv\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pps/refs/heads/main/security/pps-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Online Video
- Video Streaming
- Media and Entertainment
- Consumer
- China
- iQIYI
---
