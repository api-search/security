---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: soundhound.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: houndify.com
  spf: true
hosts:
- cert_expires: Sep  9 03:31:58 2026 GMT
  host: www.soundhound.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 28 18:49:56 2026 GMT
  host: api.houndify.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- host: api.soundhound.com
  https: false
kind: domain-security
layout: security
method: probed
name: Soundhound Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SoundHound, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SoundHound
provider_slug: soundhound
slug: soundhound-domain-security
source_filename: soundhound-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.soundhound.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 03:31:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.houndify.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 28 18:49:56 2026 GMT\n  hsts: null\n- host: api.soundhound.com\n  https: false\ndomains:\n- domain: soundhound.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: houndify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soundhound/refs/heads/main/security/soundhound-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Voice AI
- Conversational AI
- Music Recognition
- Audio Intelligence
- Speech Recognition
- Natural Language Processing
---
