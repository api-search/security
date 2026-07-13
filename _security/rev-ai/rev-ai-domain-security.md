---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rev.ai
  spf: true
hosts:
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: www.rev.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 12:51:26 2026 GMT
  host: docs.rev.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: api.rev.ai
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Rev Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rev AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Rev AI
provider_slug: rev-ai
slug: rev-ai-domain-security
source_filename: rev-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rev.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 19 23:59:59 2027 GMT\n  hsts: false\n- host: docs.rev.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 12:51:26 2026 GMT\n  hsts: false\n- host: api.rev.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: rev.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rev-ai/refs/heads/main/security/rev-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Speech Recognition
- Speech-to-Text
- Transcription
- Audio
- Natural Language Processing
- Streaming
- Real-Time
- Sentiment Analysis
- Topic Extraction
- Language Identification
---
