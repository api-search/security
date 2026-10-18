---
api_specs:
- filename: bonsai-io-clusters-api-openapi.yml
  format: yaml
  label: Bonsai Clusters API
  slug: bonsai-io-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonsai-io/refs/heads/main/openapi/bonsai-io-clusters-api-openapi.yml
- filename: bonsai-io-plans-api-openapi.yml
  format: yaml
  label: Bonsai Plans API
  slug: bonsai-io-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonsai-io/refs/heads/main/openapi/bonsai-io-plans-api-openapi.yml
- filename: bonsai-io-releases-api-openapi.yml
  format: yaml
  label: Bonsai Releases API
  slug: bonsai-io-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonsai-io/refs/heads/main/openapi/bonsai-io-releases-api-openapi.yml
- filename: bonsai-io-spaces-api-openapi.yml
  format: yaml
  label: Bonsai Spaces API
  slug: bonsai-io-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonsai-io/refs/heads/main/openapi/bonsai-io-spaces-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bonsai.io
  spf: true
hosts:
- cert_expires: Nov 20 21:31:24 2026 GMT
  host: bonsai.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bonsai Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bonsai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bonsai
provider_slug: bonsai-io
slug: bonsai-io-domain-security
source_filename: bonsai-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bonsai.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 21:31:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bonsai.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bonsai-io/refs/heads/main/security/bonsai-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Search
- Elasticsearch
- OpenSearch
- Managed Service
- Vector Search
- Cloud Infrastructure
---
