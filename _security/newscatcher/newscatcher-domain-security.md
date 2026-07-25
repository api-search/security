---
api_specs:
- filename: newscatcher-aggregationcount-api-openapi.yml
  format: yaml
  label: Newscatcher AggregationCount API
  slug: newscatcher-aggregationcount-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-aggregationcount-api-openapi.yml
- filename: newscatcher-authors-api-openapi.yml
  format: yaml
  label: Newscatcher Authors API
  slug: newscatcher-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-authors-api-openapi.yml
- filename: newscatcher-breakingnews-api-openapi.yml
  format: yaml
  label: Newscatcher BreakingNews API
  slug: newscatcher-breakingnews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-breakingnews-api-openapi.yml
- filename: newscatcher-datasets-api-openapi.yml
  format: yaml
  label: Newscatcher Datasets API
  slug: newscatcher-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-datasets-api-openapi.yml
- filename: newscatcher-entities-api-openapi.yml
  format: yaml
  label: Newscatcher Entities API
  slug: newscatcher-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-entities-api-openapi.yml
- filename: newscatcher-jobs-api-openapi.yml
  format: yaml
  label: Newscatcher Jobs API
  slug: newscatcher-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-jobs-api-openapi.yml
- filename: newscatcher-latestheadlines-api-openapi.yml
  format: yaml
  label: Newscatcher LatestHeadlines API
  slug: newscatcher-latestheadlines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-latestheadlines-api-openapi.yml
- filename: newscatcher-meta-api-openapi.yml
  format: yaml
  label: Newscatcher Meta API
  slug: newscatcher-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-meta-api-openapi.yml
- filename: newscatcher-monitors-api-openapi.yml
  format: yaml
  label: Newscatcher Monitors API
  slug: newscatcher-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-monitors-api-openapi.yml
- filename: newscatcher-projects-api-openapi.yml
  format: yaml
  label: Newscatcher Projects API
  slug: newscatcher-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-projects-api-openapi.yml
- filename: newscatcher-search-api-openapi.yml
  format: yaml
  label: Newscatcher Search API
  slug: newscatcher-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-search-api-openapi.yml
- filename: newscatcher-searchby-api-openapi.yml
  format: yaml
  label: Newscatcher SearchBy API
  slug: newscatcher-searchby-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-searchby-api-openapi.yml
- filename: newscatcher-searchbylink-api-openapi.yml
  format: yaml
  label: Newscatcher SearchByLink API
  slug: newscatcher-searchbylink-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-searchbylink-api-openapi.yml
- filename: newscatcher-sources-api-openapi.yml
  format: yaml
  label: Newscatcher Sources API
  slug: newscatcher-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-sources-api-openapi.yml
- filename: newscatcher-subscription-api-openapi.yml
  format: yaml
  label: Newscatcher Subscription API
  slug: newscatcher-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-subscription-api-openapi.yml
- filename: newscatcher-webhooks-api-openapi.yml
  format: yaml
  label: Newscatcher Webhooks API
  slug: newscatcher-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscatcher/refs/heads/main/openapi/newscatcher-webhooks-api-openapi.yml
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
