---
api_specs:
- filename: orama-openapi.yml
  format: yaml
  label: Orama Cloud Indexes and Collections
  slug: indexes-collections
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orama/refs/heads/main/openapi/orama-openapi.yml
- filename: orama-openapi.yml
  format: yaml
  label: Orama Cloud Documents
  slug: documents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orama/refs/heads/main/openapi/orama-openapi.yml
- filename: orama-openapi.yml
  format: yaml
  label: Orama Cloud Search
  slug: search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orama/refs/heads/main/openapi/orama-openapi.yml
- filename: orama-openapi.yml
  format: yaml
  label: Orama Cloud Answer Sessions (RAG)
  slug: answer-sessions-rag
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orama/refs/heads/main/openapi/orama-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: orama.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: askorama.ai
  spf: true
hosts:
- cert_expires: Oct  6 01:44:52 2026 GMT
  host: orama.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 01:16:06 2026 GMT
  host: docs.orama.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 19:39:04 2026 GMT
  host: api.askorama.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Orama Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orama, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Orama
provider_slug: orama
slug: orama-domain-security
source_filename: orama-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orama.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 01:44:52 2026 GMT\n  hsts: false\n- host: docs.orama.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 01:16:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.askorama.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 19:39:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: orama.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: askorama.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orama/refs/heads/main/security/orama-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Search
- Vector Search
- RAG
- Open Source
- Search as a Service
---
