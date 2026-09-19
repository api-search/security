---
api_specs:
- filename: api-league-art-api-openapi.yml
  format: yaml
  label: API League Art API
  slug: api-league-art-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-league/refs/heads/main/openapi/api-league-art-api-openapi.yml
- filename: api-league-books-api-openapi.yml
  format: yaml
  label: API League Books API
  slug: api-league-books-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-league/refs/heads/main/openapi/api-league-books-api-openapi.yml
- filename: api-league-food-api-openapi.yml
  format: yaml
  label: API League Food API
  slug: api-league-food-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-league/refs/heads/main/openapi/api-league-food-api-openapi.yml
- filename: api-league-games-api-openapi.yml
  format: yaml
  label: API League Games API
  slug: api-league-games-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-league/refs/heads/main/openapi/api-league-games-api-openapi.yml
- filename: api-league-humor-api-openapi.yml
  format: yaml
  label: API League Humor API
  slug: api-league-humor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-league/refs/heads/main/openapi/api-league-humor-api-openapi.yml
- filename: api-league-knowledge-api-openapi.yml
  format: yaml
  label: API League Knowledge API
  slug: api-league-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-league/refs/heads/main/openapi/api-league-knowledge-api-openapi.yml
- filename: api-league-math-api-openapi.yml
  format: yaml
  label: API League Math API
  slug: api-league-math-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-league/refs/heads/main/openapi/api-league-math-api-openapi.yml
- filename: api-league-media-api-openapi.yml
  format: yaml
  label: API League Media API
  slug: api-league-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-league/refs/heads/main/openapi/api-league-media-api-openapi.yml
- filename: api-league-news-api-openapi.yml
  format: yaml
  label: API League News API
  slug: api-league-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-league/refs/heads/main/openapi/api-league-news-api-openapi.yml
- filename: api-league-storage-api-openapi.yml
  format: yaml
  label: API League Storage API
  slug: api-league-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-league/refs/heads/main/openapi/api-league-storage-api-openapi.yml
- filename: api-league-text-api-openapi.yml
  format: yaml
  label: API League Text API
  slug: api-league-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-league/refs/heads/main/openapi/api-league-text-api-openapi.yml
- filename: api-league-web-api-openapi.yml
  format: yaml
  label: API League Web API
  slug: api-league-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-league/refs/heads/main/openapi/api-league-web-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apileague.com
  spf: true
hosts:
- cert_expires: Nov 14 20:02:43 2026 GMT
  host: apileague.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 29 09:23:25 2026 GMT
  host: api.apileague.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Api League Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for API League, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: API League
provider_slug: api-league
slug: api-league-domain-security
source_filename: api-league-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apileague.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 20:02:43 2026 GMT\n  hsts: false\n- host: api.apileague.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 09:23:25 2026 GMT\n  hsts: null\ndomains:\n- domain: apileague.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-league/refs/heads/main/security/api-league-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- API Marketplace
- Books
- Developer Tools
- Food
- Humor
- News
- SDK
- Text Processing
---
