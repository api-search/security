---
api_specs:
- filename: felt-comments-api-openapi.yml
  format: yaml
  label: Felt Comments API
  slug: felt-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/felt/refs/heads/main/openapi/felt-comments-api-openapi.yml
- filename: felt-elements-api-openapi.yml
  format: yaml
  label: Felt Elements API
  slug: felt-elements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/felt/refs/heads/main/openapi/felt-elements-api-openapi.yml
- filename: felt-embed-tokens-api-openapi.yml
  format: yaml
  label: Felt Embed Tokens API
  slug: felt-embed-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/felt/refs/heads/main/openapi/felt-embed-tokens-api-openapi.yml
- filename: felt-layer-exports-api-openapi.yml
  format: yaml
  label: Felt Layer Exports API
  slug: felt-layer-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/felt/refs/heads/main/openapi/felt-layer-exports-api-openapi.yml
- filename: felt-layer-library-api-openapi.yml
  format: yaml
  label: Felt Layer Library API
  slug: felt-layer-library-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/felt/refs/heads/main/openapi/felt-layer-library-api-openapi.yml
- filename: felt-layer-uploads-api-openapi.yml
  format: yaml
  label: Felt Layer Uploads API
  slug: felt-layer-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/felt/refs/heads/main/openapi/felt-layer-uploads-api-openapi.yml
- filename: felt-layers-api-openapi.yml
  format: yaml
  label: Felt Layers API
  slug: felt-layers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/felt/refs/heads/main/openapi/felt-layers-api-openapi.yml
- filename: felt-maps-api-openapi.yml
  format: yaml
  label: Felt Maps API
  slug: felt-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/felt/refs/heads/main/openapi/felt-maps-api-openapi.yml
- filename: felt-projects-api-openapi.yml
  format: yaml
  label: Felt Projects API
  slug: felt-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/felt/refs/heads/main/openapi/felt-projects-api-openapi.yml
- filename: felt-sources-api-openapi.yml
  format: yaml
  label: Felt Sources API
  slug: felt-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/felt/refs/heads/main/openapi/felt-sources-api-openapi.yml
- filename: felt-users-api-openapi.yml
  format: yaml
  label: Felt Users API
  slug: felt-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/felt/refs/heads/main/openapi/felt-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: felt.com
  spf: true
hosts:
- cert_expires: Aug 21 03:57:37 2026 GMT
  host: felt.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 15:35:33 2026 GMT
  host: developers.felt.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Felt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Felt, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Felt
provider_slug: felt
slug: felt-domain-security
source_filename: felt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: felt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 03:57:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.felt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 15:35:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: felt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/felt/refs/heads/main/security/felt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Maps
- GIS
- Geospatial
- Collaborative
- Mapping
- Layers
- Embedding
---
