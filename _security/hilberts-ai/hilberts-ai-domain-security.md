---
api_specs:
- filename: hilberts-ai-program-api-openapi.yml
  format: yaml
  label: Hilbert's Program API
  slug: hilberts-program-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hilberts-ai/refs/heads/main/openapi/hilberts-ai-program-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hilberts.ai
  spf: true
hosts:
- cert_expires: Sep 16 19:48:22 2026 GMT
  host: hilberts.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 00:11:05 2026 GMT
  host: app-api.hilberts.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hilberts Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hilbert''s AI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hilbert's AI
provider_slug: hilberts-ai
slug: hilberts-ai-domain-security
source_filename: hilberts-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hilberts.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 19:48:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app-api.hilberts.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 00:11:05 2026 GMT\n  hsts: null\ndomains:\n- domain: hilberts.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hilberts-ai/refs/heads/main/security/hilberts-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Growth
- Analytics
- Marketing
- Data Science
- Automation
- Agentic AI
- B2C
---
