---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: audacyinc.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: audacy.com
  spf: true
hosts:
- cert_expires: Sep 15 06:48:11 2026 GMT
  host: www.audacyinc.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 16 22:12:58 2027 GMT
  host: www.audacy.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 18:31:01 2026 GMT
  host: amperwave.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Audacy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Audacy, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Audacy
provider_slug: audacy
slug: audacy-domain-security
source_filename: audacy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.audacyinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 06:48:11 2026 GMT\n  hsts: false\n- host: www.audacy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 22:12:58 2027 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: amperwave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 18:31:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: audacyinc.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: audacy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/audacy/refs/heads/main/security/audacy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Audio
- Radio
- Podcasts
- Streaming
- Broadcasting
- Media
- Advertising
- Content
- Sports
- News
- Music
- Entertainment
- Audio Advertising
- Ad Tech
- Programmatic Audio
- Audacy
- Entercom
- Post Bankruptcy
- Privately Held
- Amperwave
- Cadence13
- Pineapple Street Studios
- Podcorn
- BetMGM Network
- Creator Lab
---
