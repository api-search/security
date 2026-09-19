---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aiola.ai
  spf: true
hosts:
- cert_expires: Oct 16 12:04:27 2026 GMT
  host: aiola.ai
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 05:25:06 2026 GMT
  host: docs.aiola.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: apis.aiola.ai
  https: false
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Aiola Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for aiOla, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: aiOla
provider_slug: aiola
slug: aiola-domain-security
source_filename: aiola-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aiola.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 12:04:27 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: docs.aiola.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 05:25:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: apis.aiola.ai\n  https: false\ndomains:\n- domain: aiola.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aiola/refs/heads/main/security/aiola-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Speech Recognition
- Speech-to-Text
- Text-to-Speech
- Voice AI
- Conversational AI
- Artificial Intelligence
- Machine-Learning
- Audio
- Transcription
- Enterprise
---
