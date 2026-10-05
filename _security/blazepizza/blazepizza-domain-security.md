---
api_specs:
- filename: blazepizza-blazepizza-api-api-openapi.yml
  format: yaml
  label: Blazepizza Blazepizza API
  slug: blazepizza-blazepizza-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blazepizza/refs/heads/main/openapi/blazepizza-blazepizza-api-api-openapi.yml
- filename: blazepizza-cat-pic-api-openapi.yml
  format: yaml
  label: Blazepizza Cat Pic API
  slug: blazepizza-cat-pic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blazepizza/refs/heads/main/openapi/blazepizza-cat-pic-api-openapi.yml
- filename: blazepizza-foo-api-openapi.yml
  format: yaml
  label: Blazepizza Foo API
  slug: blazepizza-foo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blazepizza/refs/heads/main/openapi/blazepizza-foo-api-openapi.yml
- filename: blazepizza-http-api-openapi.yml
  format: yaml
  label: Blazepizza HTTP API
  slug: blazepizza-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blazepizza/refs/heads/main/openapi/blazepizza-http-api-openapi.yml
- filename: blazepizza-image-api-openapi.yml
  format: yaml
  label: Blazepizza Image API
  slug: blazepizza-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blazepizza/refs/heads/main/openapi/blazepizza-image-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: blazepizza.com
  spf: true
hosts:
- cert_expires: Nov 11 13:28:06 2026 GMT
  host: www.blazepizza.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blazepizza Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blazepizza, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Blazepizza
provider_slug: blazepizza
slug: blazepizza-domain-security
source_filename: blazepizza-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.blazepizza.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 13:28:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: blazepizza.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blazepizza/refs/heads/main/security/blazepizza-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fast Casual
- Pizza
- Restaurant
- Franchise
---
