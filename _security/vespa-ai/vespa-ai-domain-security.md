---
api_specs:
- filename: vespa-query-api-openapi.yml
  format: yaml
  label: Vespa Query API
  slug: vespa-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vespa-ai/refs/heads/main/openapi/vespa-query-api-openapi.yml
- filename: vespa-document-api-openapi.yml
  format: yaml
  label: Vespa Document API
  slug: vespa-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vespa-ai/refs/heads/main/openapi/vespa-document-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vespa.ai
  spf: true
hosts:
- cert_expires: Sep  4 20:49:03 2026 GMT
  host: vespa.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 12 23:59:59 2027 GMT
  host: docs.vespa.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vespa Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vespa, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Vespa
provider_slug: vespa-ai
slug: vespa-ai-domain-security
source_filename: vespa-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vespa.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 20:49:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.vespa.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 12 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: vespa.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vespa-ai/refs/heads/main/security/vespa-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Search
- Vector Database
- Big Data
- Machine Learning
- Semantic Search
- Retrieval Augmented Generation
- Open Source
- Tensor
- Recommendations
---
