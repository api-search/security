---
api_specs:
- filename: kugelaudio-tts-openapi-original.json
  format: json
  label: KugelAudio TTS API
  slug: tts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kugelaudio/refs/heads/main/openapi/kugelaudio-tts-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: kugelaudio.com
  spf: true
hosts:
- cert_expires: Oct 16 00:54:29 2026 GMT
  host: www.kugelaudio.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 13:04:24 2026 GMT
  host: docs.kugelaudio.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 00:54:29 2026 GMT
  host: api.kugelaudio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kugelaudio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KugelAudio, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: KugelAudio
provider_slug: kugelaudio
slug: kugelaudio-domain-security
source_filename: kugelaudio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kugelaudio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 00:54:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.kugelaudio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 13:04:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.kugelaudio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 00:54:29 2026 GMT\n  hsts: null\ndomains:\n- domain: kugelaudio.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kugelaudio/refs/heads/main/security/kugelaudio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Voice
- Text to Speech
- Speech Synthesis
- Voice AI
- Voice Cloning
- Audio
- Artificial Intelligence
- Machine Learning
- Streaming
- Real Time
- Conversational AI
- Europe
- Data Sovereignty
- GDPR
- Company
---
