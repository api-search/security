---
api_specs:
- filename: kitforai-batch-api-openapi.yml
  format: yaml
  label: Kit For AI Batch API
  slug: kitforai-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kitforai/refs/heads/main/openapi/kitforai-batch-api-openapi.yml
- filename: kitforai-convert-api-openapi.yml
  format: yaml
  label: Kit For AI Convert API
  slug: kitforai-convert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kitforai/refs/heads/main/openapi/kitforai-convert-api-openapi.yml
- filename: kitforai-knowledge-bases-api-openapi.yml
  format: yaml
  label: Kit For AI Knowledge Bases API
  slug: kitforai-knowledge-bases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kitforai/refs/heads/main/openapi/kitforai-knowledge-bases-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kitforai.com
  spf: true
hosts:
- cert_expires: Nov 26 23:15:21 2026 GMT
  host: kitforai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kitforai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kit For AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Kit For AI
provider_slug: kitforai
slug: kitforai-domain-security
source_filename: kitforai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kitforai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 23:15:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kitforai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kitforai/refs/heads/main/security/kitforai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- AI
- Memory
- DocumentConversion
- RetrievalAugmentedGeneration
- KnowledgeBase
---
