---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dolby.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dolby.com
  spf: true
hosts:
- cert_expires: Aug 25 10:57:17 2026 GMT
  host: dolby.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 21:41:38 2026 GMT
  host: optiview.dolby.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dolby Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dolby, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dolby
provider_slug: dolby
slug: dolby-domain-security
source_filename: dolby-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dolby.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 10:57:17 2026 GMT\n  hsts: false\n- host: optiview.dolby.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 21:41:38 2026 GMT\n  hsts: false\ndomains:\n- domain: dolby.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: dolby.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dolby/refs/heads/main/security/dolby-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Audio
- Video
- Streaming
- Media
- Real-Time
---
