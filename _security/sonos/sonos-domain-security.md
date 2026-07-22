---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazonaws.com"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sonos.com
  spf: true
hosts:
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: www.sonos.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 22:28:14 2026 GMT
  host: docs.sonos.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: api.ws.sonos.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sonos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sonos, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sonos
provider_slug: sonos
slug: sonos-domain-security
source_filename: sonos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sonos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: null\n- host: docs.sonos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 22:28:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ws.sonos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sonos.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sonos/refs/heads/main/security/sonos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Audio
- Music
- Smart Home
- IoT
- Streaming
- Speakers
- Home Automation
- Voice
---
