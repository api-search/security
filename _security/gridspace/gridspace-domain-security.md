---
api_specs:
- filename: gridspace-guava-openapi.yml
  format: yaml
  label: Guava Voice Agent REST API
  slug: guava-voice-agent-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gridspace/refs/heads/main/openapi/gridspace-guava-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: goguava.ai
  spf: true
hosts:
- cert_expires: Aug 25 04:41:35 2026 GMT
  host: goguava.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.goguava.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Gridspace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gridspace, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Gridspace
provider_slug: gridspace
slug: gridspace-domain-security
source_filename: gridspace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: goguava.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 04:41:35 2026 GMT\n  hsts: false\n- host: api.goguava.ai\n  https: false\ndomains:\n- domain: goguava.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gridspace/refs/heads/main/security/gridspace-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Voice AI
- Conversational AI
- Voice Agents
- Speech Recognition
- Telephony
- SMS
- Contact Center
- Regulated Industries
- Healthcare
---
