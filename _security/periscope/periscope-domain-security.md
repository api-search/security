---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pscp.tv
  spf: true
hosts:
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: www.pscp.tv
  hsts: true
  hsts_max_age: 10886400000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Periscope Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Periscope, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Periscope
provider_slug: periscope
slug: periscope-domain-security
source_filename: periscope-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pscp.tv\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 10886400000\ndomains:\n- domain: pscp.tv\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/periscope/refs/heads/main/security/periscope-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Consumer
- Live Streaming
- Video
- Mobile
- Social
- Discontinued
---
