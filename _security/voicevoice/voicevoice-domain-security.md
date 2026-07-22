---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: maestroconference.com
  spf: false
hosts:
- cert_expires: Aug 31 23:48:00 2026 GMT
  host: maestroconference.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Voicevoice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VoiceVoice, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: VoiceVoice
provider_slug: voicevoice
slug: voicevoice-domain-security
source_filename: voicevoice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: maestroconference.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 31 23:48:00 2026 GMT\n  hsts: false\ndomains:\n- domain: maestroconference.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voicevoice/refs/heads/main/security/voicevoice-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Conferencing
- Audio
- Communications
- Defunct
---
