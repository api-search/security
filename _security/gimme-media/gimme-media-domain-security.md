---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gimmeradio.com
  spf: true
hosts:
- cert_expires: Jan 21 05:03:28 2027 GMT
  host: gimmeradio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gimme Media Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gimme Media, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Gimme Media
provider_slug: gimme-media
slug: gimme-media-domain-security
source_filename: gimme-media-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gimmeradio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 05:03:28 2027 GMT\n  hsts: null\ndomains:\n- domain: gimmeradio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gimme-media/refs/heads/main/security/gimme-media-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Music
- Streaming
- Media
- Radio
- Metal
- Ecommerce
---
