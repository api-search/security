---
api_specs:
- filename: bland-ai-openapi.yml
  format: yaml
  label: Bland AI Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bland-ai/refs/heads/main/openapi/bland-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bland.ai
  spf: true
hosts:
- cert_expires: Aug 16 23:36:23 2026 GMT
  host: www.bland.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 14:01:38 2026 GMT
  host: docs.bland.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 23:55:14 2026 GMT
  host: api.bland.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bland Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bland AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Bland AI
provider_slug: bland-ai
slug: bland-ai-domain-security
source_filename: bland-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bland.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 23:36:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.bland.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 14:01:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.bland.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 23:55:14 2026 GMT\n  hsts: null\ndomains:\n- domain: bland.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bland-ai/refs/heads/main/security/bland-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Voice
- Agents
- Phone
- Realtime
---
