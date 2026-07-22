---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: playback.tv
  spf: true
hosts:
- cert_expires: Sep 22 04:04:22 2026 GMT
  host: www.playback.tv
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Playback Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Playback, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Playback
provider_slug: playback
slug: playback-domain-security
source_filename: playback-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.playback.tv\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 04:04:22 2026 GMT\n  hsts: null\ndomains:\n- domain: playback.tv\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/playback/refs/heads/main/security/playback-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Live Streaming
- Streaming
- Video
- Creator Economy
- Entertainment
- Consumer
- Media
---
