---
api_specs:
- filename: ceramic-config-api-openapi.yml
  format: yaml
  label: Ceramic Config API
  slug: ceramic-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceramic/refs/heads/main/openapi/ceramic-config-api-openapi.yml
- filename: ceramic-debug-api-openapi.yml
  format: yaml
  label: Ceramic Debug API
  slug: ceramic-debug-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceramic/refs/heads/main/openapi/ceramic-debug-api-openapi.yml
- filename: ceramic-events-api-openapi.yml
  format: yaml
  label: Ceramic Events API
  slug: ceramic-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceramic/refs/heads/main/openapi/ceramic-events-api-openapi.yml
- filename: ceramic-experimental-api-openapi.yml
  format: yaml
  label: Ceramic Experimental API
  slug: ceramic-experimental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceramic/refs/heads/main/openapi/ceramic-experimental-api-openapi.yml
- filename: ceramic-feed-api-openapi.yml
  format: yaml
  label: Ceramic Feed API
  slug: ceramic-feed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceramic/refs/heads/main/openapi/ceramic-feed-api-openapi.yml
- filename: ceramic-interests-api-openapi.yml
  format: yaml
  label: Ceramic Interests API
  slug: ceramic-interests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceramic/refs/heads/main/openapi/ceramic-interests-api-openapi.yml
- filename: ceramic-liveness-api-openapi.yml
  format: yaml
  label: Ceramic Liveness API
  slug: ceramic-liveness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceramic/refs/heads/main/openapi/ceramic-liveness-api-openapi.yml
- filename: ceramic-peers-api-openapi.yml
  format: yaml
  label: Ceramic Peers API
  slug: ceramic-peers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceramic/refs/heads/main/openapi/ceramic-peers-api-openapi.yml
- filename: ceramic-streams-api-openapi.yml
  format: yaml
  label: Ceramic Streams API
  slug: ceramic-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceramic/refs/heads/main/openapi/ceramic-streams-api-openapi.yml
- filename: ceramic-version-api-openapi.yml
  format: yaml
  label: Ceramic Version API
  slug: ceramic-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceramic/refs/heads/main/openapi/ceramic-version-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ceramic.network
  spf: true
hosts:
- cert_expires: Aug  2 20:13:56 2026 GMT
  host: ceramic.network
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 20:45:30 2026 GMT
  host: developers.ceramic.network
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ceramic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ceramic, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Ceramic
provider_slug: ceramic
slug: ceramic-domain-security
source_filename: ceramic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ceramic.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  2 20:13:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.ceramic.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 20:45:30 2026 GMT\n  hsts: false\ndomains:\n- domain: ceramic.network\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ceramic/refs/heads/main/security/ceramic-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Decentralized
- Web3
- Data Streams
- DID
- IPFS
- Blockchain
- Event Streaming
- ComposeDB
---
