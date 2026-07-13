---
api_specs:
- filename: weaviate-openapi.yml
  format: yaml
  label: Weaviate REST API
  slug: weaviate-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weaviate/refs/heads/main/openapi/weaviate-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: weaviate.io
  spf: true
hosts:
- cert_expires: Aug 25 22:23:50 2026 GMT
  host: weaviate.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Weaviate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Weaviate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Weaviate
provider_slug: weaviate
slug: weaviate-domain-security
source_filename: weaviate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: weaviate.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 22:23:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: weaviate.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weaviate/refs/heads/main/security/weaviate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Vector Database
- AI
- Machine Learning
- Semantic Search
- Open Source
- GraphQL
- Kubernetes
---
