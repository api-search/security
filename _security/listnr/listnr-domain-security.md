---
api_specs:
- filename: listnr-openapi.yml
  format: yaml
  label: Listnr Text-to-Speech API
  slug: listnr-text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listnr/refs/heads/main/openapi/listnr-openapi.yml
- filename: listnr-openapi.yml
  format: yaml
  label: Listnr Voices API
  slug: listnr-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listnr/refs/heads/main/openapi/listnr-openapi.yml
- filename: listnr-openapi.yml
  format: yaml
  label: Listnr Audio Jobs API
  slug: listnr-audio-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listnr/refs/heads/main/openapi/listnr-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: listnr.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: listnr.tech
  spf: true
hosts:
- cert_expires: Aug 20 05:15:24 2026 GMT
  host: listnr.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 17:28:36 2026 GMT
  host: bff.listnr.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Listnr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Listnr, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Listnr
provider_slug: listnr
slug: listnr-domain-security
source_filename: listnr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: listnr.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 05:15:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: bff.listnr.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 17:28:36 2026 GMT\n  hsts: false\ndomains:\n- domain: listnr.ai\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: listnr.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/listnr/refs/heads/main/security/listnr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Text to Speech
- TTS
- Voice
- Speech Synthesis
- Audio
- Voiceover
---
