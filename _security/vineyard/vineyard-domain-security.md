---
api_specs:
- filename: vineyard-blobs-api-openapi.yml
  format: yaml
  label: Vineyard Blobs API
  slug: vineyard-blobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vineyard/refs/heads/main/openapi/vineyard-blobs-api-openapi.yml
- filename: vineyard-connection-api-openapi.yml
  format: yaml
  label: Vineyard Connection API
  slug: vineyard-connection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vineyard/refs/heads/main/openapi/vineyard-connection-api-openapi.yml
- filename: vineyard-metadata-api-openapi.yml
  format: yaml
  label: Vineyard Metadata API
  slug: vineyard-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vineyard/refs/heads/main/openapi/vineyard-metadata-api-openapi.yml
- filename: vineyard-names-api-openapi.yml
  format: yaml
  label: Vineyard Names API
  slug: vineyard-names-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vineyard/refs/heads/main/openapi/vineyard-names-api-openapi.yml
- filename: vineyard-objects-api-openapi.yml
  format: yaml
  label: Vineyard Objects API
  slug: vineyard-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vineyard/refs/heads/main/openapi/vineyard-objects-api-openapi.yml
- filename: vineyard-persistence-api-openapi.yml
  format: yaml
  label: Vineyard Persistence API
  slug: vineyard-persistence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vineyard/refs/heads/main/openapi/vineyard-persistence-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: v6d.io
  spf: false
hosts:
- cert_expires: Sep 19 07:58:51 2026 GMT
  host: v6d.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vineyard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vineyard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Vineyard
provider_slug: vineyard
slug: vineyard-domain-security
source_filename: vineyard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: v6d.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 07:58:51 2026 GMT\n  hsts: false\ndomains:\n- domain: v6d.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vineyard/refs/heads/main/security/vineyard-domain-security.yml
summary_line: TLSv1.3
tags:
- Big Data
- CNCF
- Cloud Native
- Data Engineering
- Distributed Systems
- In-Memory Storage
- Kubernetes
- Machine Learning
- Metadata Management
- Python
- Zero-Copy
---
