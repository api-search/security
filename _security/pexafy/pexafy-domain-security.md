---
api_specs:
- filename: pexafy-collections-api-openapi.yml
  format: yaml
  label: Pexafy Collections API
  slug: pexafy-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pexafy/refs/heads/main/openapi/pexafy-collections-api-openapi.yml
- filename: pexafy-facets-api-openapi.yml
  format: yaml
  label: Pexafy Facets API
  slug: pexafy-facets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pexafy/refs/heads/main/openapi/pexafy-facets-api-openapi.yml
- filename: pexafy-photos-api-openapi.yml
  format: yaml
  label: Pexafy Photos API
  slug: pexafy-photos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pexafy/refs/heads/main/openapi/pexafy-photos-api-openapi.yml
- filename: pexafy-search-api-openapi.yml
  format: yaml
  label: Pexafy Search API
  slug: pexafy-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pexafy/refs/heads/main/openapi/pexafy-search-api-openapi.yml
- filename: pexafy-usage-api-openapi.yml
  format: yaml
  label: Pexafy Usage API
  slug: pexafy-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pexafy/refs/heads/main/openapi/pexafy-usage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pexafy.com
  spf: true
hosts:
- cert_expires: Nov 17 03:58:49 2026 GMT
  cert_issuer: Google Trust Services WE1
  host: pexafy.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 08:31:23 2026 GMT
  host: api.pexafy.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 08:31:23 2026 GMT
  host: docs.pexafy.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 08:31:23 2026 GMT
  cert_issuer: Let's Encrypt YE1
  host: mcp.pexafy.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pexafy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pexafy, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pexafy
provider_slug: pexafy
slug: pexafy-domain-security
source_filename: pexafy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts (0-working/probe-domain-security.py,\n  then hand-verified with curl -I on each host)\nnote: >-\n  probe-domain-security.py recorded hsts: null for api.pexafy.com and did not visit\n  pexafy.com or mcp.pexafy.com. A direct HEAD to each host returned\n  \"strict-transport-security: max-age=31536000; includeSubDomains\" on all four, so the\n  hsts values below are the observed ones. Every host is fronted by Cloudflare in front\n  of Caddy.\nhosts:\n- host: pexafy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 03:58:49 2026 GMT\n  cert_issuer: Google Trust Services WE1\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: api.pexafy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 08:31:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: docs.pexafy.com\n  https: true\n\
  \  tls_version: TLSv1.3\n  cert_expires: Oct  8 08:31:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: mcp.pexafy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 08:31:23 2026 GMT\n  cert_issuer: Let's Encrypt YE1\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\ndomains:\n- domain: pexafy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\nresponse_headers_observed:\n  source: GET https://api.pexafy.com/health and GET https://api.pexafy.com/api/v1/search/photos (401)\n  headers:\n  - content-security-policy: \"default-src 'none'; frame-ancestors 'none'\"\n  - permissions-policy: \"camera=(), microphone=(), geolocation=()\"\n  - referrer-policy: strict-origin-when-cross-origin\n  - x-content-type-options: nosniff\n  - x-frame-options: DENY\ngaps:\n- No DNSSEC on pexafy.com.\n- No CAA records on pexafy.com.\n- DMARC policy is p=none (monitor only), not quarantine or reject.\n\
  - No /.well-known/security.txt served on any host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pexafy/refs/heads/main/security/pexafy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- images
- photos
- stock photos
- image search
- semantic search
- computer vision
- embeddings
- mcp
- agent-native
- content licensing
---
