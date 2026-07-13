---
api_specs:
- filename: celestia-blob-api-openapi.yml
  format: yaml
  label: Celestia Node Blob API
  slug: celestia-blob-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celestia/refs/heads/main/openapi/celestia-blob-api-openapi.yml
- filename: celestia-header-api-openapi.yml
  format: yaml
  label: Celestia Node Header API
  slug: celestia-header-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celestia/refs/heads/main/openapi/celestia-header-api-openapi.yml
- filename: celestia-da-api-openapi.yml
  format: yaml
  label: Celestia Node DA API
  slug: celestia-da-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celestia/refs/heads/main/openapi/celestia-da-api-openapi.yml
- filename: celestia-share-api-openapi.yml
  format: yaml
  label: Celestia Node Share API
  slug: celestia-share-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celestia/refs/heads/main/openapi/celestia-share-api-openapi.yml
- filename: celestia-state-api-openapi.yml
  format: yaml
  label: Celestia Node State API
  slug: celestia-state-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celestia/refs/heads/main/openapi/celestia-state-api-openapi.yml
- filename: celestia-das-api-openapi.yml
  format: yaml
  label: Celestia Node DAS API
  slug: celestia-das-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celestia/refs/heads/main/openapi/celestia-das-api-openapi.yml
- filename: celestia-fraud-api-openapi.yml
  format: yaml
  label: Celestia Node Fraud API
  slug: celestia-fraud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celestia/refs/heads/main/openapi/celestia-fraud-api-openapi.yml
- filename: celestia-p2p-api-openapi.yml
  format: yaml
  label: Celestia Node P2P API
  slug: celestia-p2p-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celestia/refs/heads/main/openapi/celestia-p2p-api-openapi.yml
- filename: celestia-node-api-openapi.yml
  format: yaml
  label: Celestia Node Admin API
  slug: celestia-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celestia/refs/heads/main/openapi/celestia-node-api-openapi.yml
- filename: celestia-blobstream-api-openapi.yml
  format: yaml
  label: Celestia Node Blobstream API
  slug: celestia-blobstream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celestia/refs/heads/main/openapi/celestia-blobstream-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: true
  domain: celestia.org
  spf: true
hosts:
- cert_expires: Sep 29 03:27:29 2026 GMT
  host: celestia.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: node-rpc-docs.celestia.org
  https: false
kind: domain-security
layout: security
method: probed
name: Celestia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for celestia, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present.'
provider_name: celestia
provider_slug: celestia
slug: celestia-domain-security
source_filename: celestia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: celestia.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 03:27:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: node-rpc-docs.celestia.org\n  https: false\ndomains:\n- domain: celestia.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/celestia/refs/heads/main/security/celestia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags: []
---
