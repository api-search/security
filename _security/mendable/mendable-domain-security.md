---
api_specs:
- filename: mendable-openapi.yml
  format: yaml
  label: Mendable Chat & Answers API
  slug: mendable-chat-answers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mendable/refs/heads/main/openapi/mendable-openapi.yml
- filename: mendable-openapi.yml
  format: yaml
  label: Mendable Conversations API
  slug: mendable-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mendable/refs/heads/main/openapi/mendable-openapi.yml
- filename: mendable-openapi.yml
  format: yaml
  label: Mendable Data Ingestion & Sources API
  slug: mendable-data-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mendable/refs/heads/main/openapi/mendable-openapi.yml
- filename: mendable-openapi.yml
  format: yaml
  label: Mendable Ratings API
  slug: mendable-ratings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mendable/refs/heads/main/openapi/mendable-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mendable.ai
  spf: true
hosts:
- cert_expires: Sep 20 15:27:31 2026 GMT
  host: www.mendable.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 05:07:06 2026 GMT
  host: docs.mendable.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 23:23:06 2026 GMT
  host: api.mendable.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mendable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mendable, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mendable
provider_slug: mendable
slug: mendable-domain-security
source_filename: mendable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mendable.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 15:27:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.mendable.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 05:07:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.mendable.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 23:23:06 2026 GMT\n  hsts: false\ndomains:\n- domain: mendable.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mendable/refs/heads/main/security/mendable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Answers
- Enterprise Search
- RAG
- Support
---
