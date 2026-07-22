---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tvbeat.com
  spf: true
hosts:
- cert_expires: Sep 29 06:51:03 2026 GMT
  host: tvbeat.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tvbeat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TVbeat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TVbeat
provider_slug: tvbeat
slug: tvbeat-domain-security
source_filename: tvbeat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tvbeat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 06:51:03 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: tvbeat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tvbeat/refs/heads/main/security/tvbeat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- AdTech
- Television
- Streaming
- CTV
- Audience Measurement
- Analytics
- Media
---
