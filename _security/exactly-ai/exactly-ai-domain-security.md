---
api_specs:
- filename: exactly-ai-public-openapi-original.json
  format: json
  label: Exactly Public API
  slug: exactly-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exactly-ai/refs/heads/main/openapi/exactly-ai-public-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: exactly.ai
  spf: true
hosts:
- cert_expires: Sep 23 18:54:47 2026 GMT
  host: api.exactly.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Exactly Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Exactly Ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Exactly Ai
provider_slug: exactly-ai
slug: exactly-ai-domain-security
source_filename: exactly-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.exactly.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 18:54:47 2026 GMT\n  hsts: null\ndomains:\n- domain: exactly.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exactly-ai/refs/heads/main/security/exactly-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Image Generation
- Generative AI
- Creative Tools
- Brand
- Machine Learning
- Media
---
