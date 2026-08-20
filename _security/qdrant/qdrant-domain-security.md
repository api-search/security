---
api_specs:
- filename: qdrant-aliases-api-openapi.yml
  format: yaml
  label: Qdrant Aliases API
  slug: qdrant-aliases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qdrant/refs/heads/main/openapi/qdrant-aliases-api-openapi.yml
- filename: qdrant-beta-api-openapi.yml
  format: yaml
  label: Qdrant Beta API
  slug: qdrant-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qdrant/refs/heads/main/openapi/qdrant-beta-api-openapi.yml
- filename: qdrant-collections-api-openapi.yml
  format: yaml
  label: Qdrant Collections API
  slug: qdrant-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qdrant/refs/heads/main/openapi/qdrant-collections-api-openapi.yml
- filename: qdrant-distributed-api-openapi.yml
  format: yaml
  label: Qdrant Distributed API
  slug: qdrant-distributed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qdrant/refs/heads/main/openapi/qdrant-distributed-api-openapi.yml
- filename: qdrant-indexes-api-openapi.yml
  format: yaml
  label: Qdrant Indexes API
  slug: qdrant-indexes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qdrant/refs/heads/main/openapi/qdrant-indexes-api-openapi.yml
- filename: qdrant-points-api-openapi.yml
  format: yaml
  label: Qdrant Points API
  slug: qdrant-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qdrant/refs/heads/main/openapi/qdrant-points-api-openapi.yml
- filename: qdrant-search-api-openapi.yml
  format: yaml
  label: Qdrant Search API
  slug: qdrant-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qdrant/refs/heads/main/openapi/qdrant-search-api-openapi.yml
- filename: qdrant-service-api-openapi.yml
  format: yaml
  label: Qdrant Service API
  slug: qdrant-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qdrant/refs/heads/main/openapi/qdrant-service-api-openapi.yml
- filename: qdrant-snapshots-api-openapi.yml
  format: yaml
  label: Qdrant Snapshots API
  slug: qdrant-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qdrant/refs/heads/main/openapi/qdrant-snapshots-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: qdrant.tech
  spf: true
hosts:
- cert_expires: Aug 19 21:53:49 2026 GMT
  host: qdrant.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qdrant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qdrant, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Qdrant
provider_slug: qdrant
slug: qdrant-domain-security
source_filename: qdrant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: qdrant.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 21:53:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: qdrant.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qdrant/refs/heads/main/security/qdrant-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Vector Databases
---
