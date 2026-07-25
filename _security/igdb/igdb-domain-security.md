---
api_specs:
- filename: igdb-companies-api-openapi.yml
  format: yaml
  label: IGDB Companies API
  slug: igdb-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/igdb/refs/heads/main/openapi/igdb-companies-api-openapi.yml
- filename: igdb-games-api-openapi.yml
  format: yaml
  label: IGDB Games API
  slug: igdb-games-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/igdb/refs/heads/main/openapi/igdb-games-api-openapi.yml
- filename: igdb-genres-api-openapi.yml
  format: yaml
  label: IGDB Genres API
  slug: igdb-genres-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/igdb/refs/heads/main/openapi/igdb-genres-api-openapi.yml
- filename: igdb-media-api-openapi.yml
  format: yaml
  label: IGDB Media API
  slug: igdb-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/igdb/refs/heads/main/openapi/igdb-media-api-openapi.yml
- filename: igdb-platforms-api-openapi.yml
  format: yaml
  label: IGDB Platforms API
  slug: igdb-platforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/igdb/refs/heads/main/openapi/igdb-platforms-api-openapi.yml
- filename: igdb-reference-api-openapi.yml
  format: yaml
  label: IGDB Reference API
  slug: igdb-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/igdb/refs/heads/main/openapi/igdb-reference-api-openapi.yml
- filename: igdb-releases-api-openapi.yml
  format: yaml
  label: IGDB Releases API
  slug: igdb-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/igdb/refs/heads/main/openapi/igdb-releases-api-openapi.yml
- filename: igdb-search-api-openapi.yml
  format: yaml
  label: IGDB Search API
  slug: igdb-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/igdb/refs/heads/main/openapi/igdb-search-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: igdb.com
  spf: true
hosts:
- cert_expires: Sep 21 06:12:44 2026 GMT
  host: www.igdb.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 23:59:59 2026 GMT
  host: api.igdb.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Igdb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IGDB, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: IGDB
provider_slug: igdb
slug: igdb-domain-security
source_filename: igdb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.igdb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 06:12:44 2026 GMT\n  hsts: null\n- host: api.igdb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: igdb.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/igdb/refs/heads/main/security/igdb-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Entertainment
- Game Database
- Gaming
- Video Games
---
