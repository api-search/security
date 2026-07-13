---
api_specs:
- filename: newscatcher-news-api-openapi.yml
  format: yaml
  label: Newscatcher News API
  slug: news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-news-api-openapi.yml
- filename: newscatcher-web-search-api-openapi.yml
  format: yaml
  label: Newscatcher CatchAll Web Search API
  slug: web-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-web-search-api-openapi.yml
- filename: newscatcher-local-news-api-openapi.yml
  format: yaml
  label: Newscatcher Local News API
  slug: local-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-local-news-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: newscatcherapi.com
  spf: true
hosts:
- cert_expires: Aug 11 11:44:10 2026 GMT
  host: www.newscatcherapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 20:01:59 2026 GMT
  host: v3-api.newscatcherapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.newscatcherapi.com
  https: false
kind: domain-security
layout: security
method: probed
name: Newscatcher Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Newscatcher, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Newscatcher
provider_slug: newscatcher
slug: newscatcher-domain-security
source_filename: newscatcher-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.newscatcherapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 11:44:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: v3-api.newscatcherapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 20:01:59 2026 GMT\n  hsts: null\n- host: api.newscatcherapi.com\n  https: false\ndomains:\n- domain: newscatcherapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/security/newscatcher-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- News
- Search
- NLP
- Sentiment Analysis
- Entity Extraction
- Clustering
- Media Intelligence
- Financial Intelligence
- AI
- Enterprise
---
