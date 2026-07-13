---
api_specs:
- filename: deepinfra-openapi.yml
  format: yaml
  label: DeepInfra Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepinfra/refs/heads/main/openapi/deepinfra-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: deepinfra.com
  spf: true
hosts:
- cert_expires: Aug 15 10:44:54 2026 GMT
  host: deepinfra.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 06:41:40 2026 GMT
  host: docs.deepinfra.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 22:20:35 2026 GMT
  host: api.deepinfra.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deepinfra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DeepInfra, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DeepInfra
provider_slug: deepinfra
slug: deepinfra-domain-security
source_filename: deepinfra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deepinfra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 10:44:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.deepinfra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 06:41:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.deepinfra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 22:20:35 2026 GMT\n  hsts: null\ndomains:\n- domain: deepinfra.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deepinfra/refs/heads/main/security/deepinfra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- LLM
- Inference
- Serverless
- Open Source
- OpenAI Compatible
- Anthropic Compatible
- Image Generation
- Audio
- Embeddings
---
