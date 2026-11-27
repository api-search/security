---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: meeting.ai
  spf: true
hosts:
- cert_expires: Jan  4 20:02:29 2027 GMT
  host: meeting.ai
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Meeting.ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meeting.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Meeting.ai
provider_slug: meeting-ai
slug: meeting-ai-domain-security
source_filename: meeting-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: meeting.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 20:02:29 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: meeting.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/meeting-ai/security/meeting-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Productivity
- Meeting
- Transcription
- Summarization
---
