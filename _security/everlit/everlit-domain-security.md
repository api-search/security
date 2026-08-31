---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: everlit.audio
  spf: true
hosts:
- cert_expires: Oct 11 07:26:16 2026 GMT
  host: everlit.audio
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Everlit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Everlit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Everlit
provider_slug: everlit
slug: everlit-domain-security
source_filename: everlit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: everlit.audio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 07:26:16 2026 GMT\n  hsts: false\ndomains:\n- domain: everlit.audio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/everlit/refs/heads/main/security/everlit-domain-security.yml
summary_line: TLSv1.3
tags:
- Audio
- Video
- social
- Podcasts
- Media
- publishers
- News
- text-to-speech
- AI-voice
- content-distribution
- monetization
- accessibility
- oEmbed
- embeddable-player
- Advertising
---
