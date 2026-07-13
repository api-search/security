---
api_specs:
- filename: tidal-catalog-api-openapi.yml
  format: yaml
  label: TIDAL Catalog API
  slug: tidal-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidal/refs/heads/main/openapi/tidal-catalog-api-openapi.yml
- filename: tidal-search-api-openapi.yml
  format: yaml
  label: TIDAL Search API
  slug: tidal-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidal/refs/heads/main/openapi/tidal-search-api-openapi.yml
- filename: tidal-playlists-api-openapi.yml
  format: yaml
  label: TIDAL Playlists API
  slug: tidal-playlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidal/refs/heads/main/openapi/tidal-playlists-api-openapi.yml
- filename: tidal-users-api-openapi.yml
  format: yaml
  label: TIDAL Users API
  slug: tidal-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidal/refs/heads/main/openapi/tidal-users-api-openapi.yml
- filename: tidal-user-collections-api-openapi.yml
  format: yaml
  label: TIDAL User Collections API
  slug: tidal-user-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidal/refs/heads/main/openapi/tidal-user-collections-api-openapi.yml
- filename: tidal-recommendations-api-openapi.yml
  format: yaml
  label: TIDAL Recommendations API
  slug: tidal-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidal/refs/heads/main/openapi/tidal-recommendations-api-openapi.yml
- filename: tidal-playback-api-openapi.yml
  format: yaml
  label: TIDAL Playback API
  slug: tidal-playback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidal/refs/heads/main/openapi/tidal-playback-api-openapi.yml
- filename: tidal-social-api-openapi.yml
  format: yaml
  label: TIDAL Social API
  slug: tidal-social-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidal/refs/heads/main/openapi/tidal-social-api-openapi.yml
- filename: tidal-commerce-api-openapi.yml
  format: yaml
  label: TIDAL Commerce API
  slug: tidal-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidal/refs/heads/main/openapi/tidal-commerce-api-openapi.yml
- filename: tidal-claims-api-openapi.yml
  format: yaml
  label: TIDAL Claims API
  slug: tidal-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tidal/refs/heads/main/openapi/tidal-claims-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tidal.com
  spf: true
hosts:
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: tidal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: developer.tidal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: openapi.tidal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tidal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TIDAL, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TIDAL
provider_slug: tidal
slug: tidal-domain-security
source_filename: tidal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tidal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: null\n- host: developer.tidal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: false\n- host: openapi.tidal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tidal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tidal/refs/heads/main/security/tidal-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Music
- Streaming
- Hi-Fi
- HiRes Lossless
- Audio
- Block
- Square
---
