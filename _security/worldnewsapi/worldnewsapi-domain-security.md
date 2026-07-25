---
api_specs:
- filename: worldnewsapi-extract-news-api-openapi.yml
  format: yaml
  label: World News API Extract News API
  slug: worldnewsapi-extract-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/openapi/worldnewsapi-extract-news-api-openapi.yml
- filename: worldnewsapi-front-pages-api-openapi.yml
  format: yaml
  label: World News API Front Pages API
  slug: worldnewsapi-front-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/openapi/worldnewsapi-front-pages-api-openapi.yml
- filename: worldnewsapi-geo-coordinates-api-openapi.yml
  format: yaml
  label: World News API Geo Coordinates API
  slug: worldnewsapi-geo-coordinates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/openapi/worldnewsapi-geo-coordinates-api-openapi.yml
- filename: worldnewsapi-news-sources-api-openapi.yml
  format: yaml
  label: World News API News Sources API
  slug: worldnewsapi-news-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/openapi/worldnewsapi-news-sources-api-openapi.yml
- filename: worldnewsapi-retrieve-news-api-openapi.yml
  format: yaml
  label: World News API Retrieve News API
  slug: worldnewsapi-retrieve-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/openapi/worldnewsapi-retrieve-news-api-openapi.yml
- filename: worldnewsapi-search-news-api-openapi.yml
  format: yaml
  label: World News API Search News API
  slug: worldnewsapi-search-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/openapi/worldnewsapi-search-news-api-openapi.yml
- filename: worldnewsapi-top-news-api-openapi.yml
  format: yaml
  label: World News API Top News API
  slug: worldnewsapi-top-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/openapi/worldnewsapi-top-news-api-openapi.yml
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
