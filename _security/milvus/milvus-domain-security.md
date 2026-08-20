---
api_specs:
- filename: milvus-collections-api-openapi.yml
  format: yaml
  label: Milvus Collections API
  slug: milvus-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/milvus/refs/heads/main/openapi/milvus-collections-api-openapi.yml
- filename: milvus-entities-api-openapi.yml
  format: yaml
  label: Milvus Entities API
  slug: milvus-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/milvus/refs/heads/main/openapi/milvus-entities-api-openapi.yml
- filename: milvus-indexes-api-openapi.yml
  format: yaml
  label: Milvus Indexes API
  slug: milvus-indexes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/milvus/refs/heads/main/openapi/milvus-indexes-api-openapi.yml
- filename: milvus-partitions-api-openapi.yml
  format: yaml
  label: Milvus Partitions API
  slug: milvus-partitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/milvus/refs/heads/main/openapi/milvus-partitions-api-openapi.yml
- filename: milvus-roles-api-openapi.yml
  format: yaml
  label: Milvus Roles API
  slug: milvus-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/milvus/refs/heads/main/openapi/milvus-roles-api-openapi.yml
- filename: milvus-users-api-openapi.yml
  format: yaml
  label: Milvus Users API
  slug: milvus-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/milvus/refs/heads/main/openapi/milvus-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: milvus.io
  spf: true
hosts:
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: milvus.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Milvus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Milvus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Milvus
provider_slug: milvus
slug: milvus-domain-security
source_filename: milvus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: milvus.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: milvus.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/milvus/refs/heads/main/security/milvus-domain-security.yml
summary_line: TLSv1.3
tags:
- Vector Database
- Artificial Intelligence
- Embeddings
- Open-Source
- Cloud-Native
---
