---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: comcast.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: codebig2.net
  spf: false
hosts:
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: www.comcast.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 08:54:59 2026 GMT
  host: docs.developer.comcast.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: sat-prod.codebig2.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Comcast Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Comcast, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Comcast
provider_slug: comcast
slug: comcast-domain-security
source_filename: comcast-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.comcast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: null\n- host: docs.developer.comcast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 08:54:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sat-prod.codebig2.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: comcast.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: codebig2.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/comcast/refs/heads/main/security/comcast-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cable
- Connected Devices
- Entertainment
- Internet
- Media
- Mobile
- Streaming
- Wireless
- Fortune 100
---
