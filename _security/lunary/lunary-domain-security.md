---
api_specs:
- filename: lunary-openapi.yml
  format: yaml
  label: Lunary API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunary/refs/heads/main/openapi/lunary-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lunary.ai
  spf: false
hosts:
- cert_expires: Sep 24 16:17:16 2026 GMT
  host: lunary.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 03:37:50 2026 GMT
  host: docs.lunary.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 03:34:59 2026 GMT
  host: api.lunary.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lunary Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lunary, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Lunary
provider_slug: lunary
slug: lunary-domain-security
source_filename: lunary-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lunary.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 16:17:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.lunary.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 03:37:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.lunary.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 03:34:59 2026 GMT\n  hsts: null\ndomains:\n- domain: lunary.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lunary/refs/heads/main/security/lunary-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Evaluation
- Observability
- Open Source
- LLM
- Tracing
- Prompts
---
