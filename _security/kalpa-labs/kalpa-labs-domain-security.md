---
api_specs:
- filename: kalpa-labs-openapi-original.json
  format: json
  label: Kalpa Speech API
  slug: kalpa-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kalpa-labs/refs/heads/main/openapi/kalpa-labs-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kalpalabs.ai
  spf: true
hosts:
- cert_expires: Oct 13 22:55:43 2026 GMT
  host: api.kalpalabs.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kalpa Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kalpa Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kalpa Labs
provider_slug: kalpa-labs
slug: kalpa-labs-domain-security
source_filename: kalpa-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.kalpalabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 22:55:43 2026 GMT\n  hsts: null\ndomains:\n- domain: kalpalabs.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kalpa-labs/refs/heads/main/security/kalpa-labs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Speech
- Text to Speech
- Voice
- Audio
- Conversational AI
- Machine Learning
- Artificial Intelligence
---
