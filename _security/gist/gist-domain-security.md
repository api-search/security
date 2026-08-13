---
api_specs:
- filename: gist-answers-api-openapi.yml
  format: yaml
  label: Gist Answers API (Prorata API Service)
  slug: gist-answers-api-prorata-api-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gist/refs/heads/main/openapi/gist-answers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gist.ai
  spf: true
hosts:
- cert_expires: Nov 10 02:33:31 2026 GMT
  host: gist.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 12:31:12 2026 GMT
  host: platform.gist.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 10:40:20 2026 GMT
  host: api.gist.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gist, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gist
provider_slug: gist
slug: gist-domain-security
source_filename: gist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gist.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 02:33:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: platform.gist.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 12:31:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.gist.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 10:40:20 2026 GMT\n  hsts: null\ndomains:\n- domain: gist.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gist/refs/heads/main/security/gist-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Generative AI
- Advertising
- Marketing
- Brand Visibility
- Publishers
- Search
- Content
- Answer Engine
- Attribution
- Content Licensing
- Media
- RAG
- Advertising Technology
---
