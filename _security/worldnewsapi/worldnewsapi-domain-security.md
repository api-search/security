---
api_specs:
- filename: worldnewsapi-openapi.yml
  format: yaml
  label: World News Search News API
  slug: worldnewsapi-search-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/openapi/worldnewsapi-openapi.yml
- filename: worldnewsapi-openapi.yml
  format: yaml
  label: World News Geo Coordinates API
  slug: worldnewsapi-geo-coordinates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/openapi/worldnewsapi-openapi.yml
- filename: worldnewsapi-openapi.yml
  format: yaml
  label: World News Top News API
  slug: worldnewsapi-top-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/openapi/worldnewsapi-openapi.yml
- filename: worldnewsapi-openapi.yml
  format: yaml
  label: World News Extract News API
  slug: worldnewsapi-extract-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/openapi/worldnewsapi-openapi.yml
- filename: worldnewsapi-openapi.yml
  format: yaml
  label: World News Retrieve News API
  slug: worldnewsapi-retrieve-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/openapi/worldnewsapi-openapi.yml
- filename: worldnewsapi-openapi.yml
  format: yaml
  label: World News Sources API
  slug: worldnewsapi-news-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/openapi/worldnewsapi-openapi.yml
- filename: worldnewsapi-openapi.yml
  format: yaml
  label: World News Front Pages API
  slug: worldnewsapi-front-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/openapi/worldnewsapi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: worldnewsapi.com
  spf: false
hosts:
- host: worldnewsapi.com
  hsts: false
  https: true
  server: cloudflare
  tls_version: TLSv1.3
- cert_expires: Sep 22 10:18:54 2026 GMT
  host: api.worldnewsapi.com
  hsts: false
  https: true
  server: cloudflare
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Worldnewsapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for World News API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: World News API
provider_slug: worldnewsapi
slug: worldnewsapi-domain-security
source_filename: worldnewsapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: worldnewsapi.com\n  https: true\n  tls_version: TLSv1.3\n  server: cloudflare\n  hsts: false\n- host: api.worldnewsapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 10:18:54 2026 GMT\n  server: cloudflare\n  hsts: false\ndomains:\n- domain: worldnewsapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/security/worldnewsapi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- News
- Local News
- News Search
- Media Monitoring
- Geo Search
- News Data
- Sentiment Analysis
- Content Extraction
---
