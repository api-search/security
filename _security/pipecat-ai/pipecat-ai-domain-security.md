---
api_specs:
- filename: pipecat-ai-openapi.yml
  format: yaml
  label: Pipecat Cloud (Agents/Sessions API)
  slug: pipecat-cloud-agents-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pipecat-ai/refs/heads/main/openapi/pipecat-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pipecat.ai
  spf: true
- caa:
  - 0 iodef "mailto:help@daily.co"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: daily.co
  spf: true
hosts:
- cert_expires: Aug 12 03:25:21 2026 GMT
  host: www.pipecat.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 18:31:11 2026 GMT
  host: docs.pipecat.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: api.pipecat.daily.co
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Pipecat Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pipecat, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Pipecat
provider_slug: pipecat-ai
slug: pipecat-ai-domain-security
source_filename: pipecat-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pipecat.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 03:25:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.pipecat.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 18:31:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.pipecat.daily.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: pipecat.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: daily.co\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:help@daily.co\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pipecat-ai/refs/heads/main/security/pipecat-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Voice
- Multimodal
- Agents
- Realtime
- Framework
---
