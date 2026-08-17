---
api_specs:
- filename: newswhip-articles-api-openapi.yml
  format: yaml
  label: NewsWhip Articles API
  slug: newswhip-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newswhip/refs/heads/main/openapi/newswhip-articles-api-openapi.yml
- filename: newswhip-articlesbyhrefs-api-openapi.yml
  format: yaml
  label: NewsWhip ArticlesByHrefs API
  slug: newswhip-articlesbyhrefs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newswhip/refs/heads/main/openapi/newswhip-articlesbyhrefs-api-openapi.yml
- filename: newswhip-content-api-openapi.yml
  format: yaml
  label: NewsWhip Content API
  slug: newswhip-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newswhip/refs/heads/main/openapi/newswhip-content-api-openapi.yml
- filename: newswhip-fbinfluencers-api-openapi.yml
  format: yaml
  label: NewsWhip FbInfluencers API
  slug: newswhip-fbinfluencers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newswhip/refs/heads/main/openapi/newswhip-fbinfluencers-api-openapi.yml
- filename: newswhip-fbposts-api-openapi.yml
  format: yaml
  label: NewsWhip FbPosts API
  slug: newswhip-fbposts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newswhip/refs/heads/main/openapi/newswhip-fbposts-api-openapi.yml
- filename: newswhip-influencers-api-openapi.yml
  format: yaml
  label: NewsWhip Influencers API
  slug: newswhip-influencers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newswhip/refs/heads/main/openapi/newswhip-influencers-api-openapi.yml
- filename: newswhip-local-api-openapi.yml
  format: yaml
  label: NewsWhip Local API
  slug: newswhip-local-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newswhip/refs/heads/main/openapi/newswhip-local-api-openapi.yml
- filename: newswhip-publisher-api-openapi.yml
  format: yaml
  label: NewsWhip Publisher API
  slug: newswhip-publisher-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newswhip/refs/heads/main/openapi/newswhip-publisher-api-openapi.yml
- filename: newswhip-rankings-api-openapi.yml
  format: yaml
  label: NewsWhip Rankings API
  slug: newswhip-rankings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newswhip/refs/heads/main/openapi/newswhip-rankings-api-openapi.yml
- filename: newswhip-region-api-openapi.yml
  format: yaml
  label: NewsWhip Region API
  slug: newswhip-region-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newswhip/refs/heads/main/openapi/newswhip-region-api-openapi.yml
- filename: newswhip-search-api-openapi.yml
  format: yaml
  label: NewsWhip Search API
  slug: newswhip-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newswhip/refs/heads/main/openapi/newswhip-search-api-openapi.yml
- filename: newswhip-social-api-openapi.yml
  format: yaml
  label: NewsWhip Social API
  slug: newswhip-social-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newswhip/refs/heads/main/openapi/newswhip-social-api-openapi.yml
- filename: newswhip-statistics-api-openapi.yml
  format: yaml
  label: NewsWhip Statistics API
  slug: newswhip-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newswhip/refs/heads/main/openapi/newswhip-statistics-api-openapi.yml
- filename: newswhip-stats-api-openapi.yml
  format: yaml
  label: NewsWhip Stats API
  slug: newswhip-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newswhip/refs/heads/main/openapi/newswhip-stats-api-openapi.yml
- filename: newswhip-twitterinfluencers-api-openapi.yml
  format: yaml
  label: NewsWhip TwitterInfluencers API
  slug: newswhip-twitterinfluencers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newswhip/refs/heads/main/openapi/newswhip-twitterinfluencers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: newswhip.com
  spf: true
hosts:
- cert_expires: Nov  8 18:56:13 2026 GMT
  host: newswhip.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 14:16:27 2026 GMT
  host: developer.newswhip.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 19:12:54 2026 GMT
  host: api.newswhip.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Newswhip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NewsWhip, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NewsWhip
provider_slug: newswhip
slug: newswhip-domain-security
source_filename: newswhip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: newswhip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 18:56:13 2026 GMT\n  hsts: false\n- host: developer.newswhip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 14:16:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.newswhip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 19:12:54 2026 GMT\n  hsts: null\ndomains:\n- domain: newswhip.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newswhip/refs/heads/main/security/newswhip-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Media Intelligence
- Social Media Analytics
- News
- Content Analytics
- Engagement Data
- Predictive Analytics
- Media Monitoring
---
