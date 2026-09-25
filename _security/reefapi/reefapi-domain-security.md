---
api_specs:
- filename: reefapi-classifieds-second-hand-api-openapi.yml
  format: yaml
  label: ReefAPI Classifieds & Second-hand API
  slug: reefapi-classifieds-second-hand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reefapi/refs/heads/main/openapi/reefapi-classifieds-second-hand-api-openapi.yml
- filename: reefapi-developer-tools-api-openapi.yml
  format: yaml
  label: ReefAPI Developer Tools API
  slug: reefapi-developer-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reefapi/refs/heads/main/openapi/reefapi-developer-tools-api-openapi.yml
- filename: reefapi-e-commerce-marketplaces-api-openapi.yml
  format: yaml
  label: ReefAPI E-commerce & Marketplaces API
  slug: reefapi-e-commerce-marketplaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reefapi/refs/heads/main/openapi/reefapi-e-commerce-marketplaces-api-openapi.yml
- filename: reefapi-finance-data-api-openapi.yml
  format: yaml
  label: ReefAPI Finance & Data API
  slug: reefapi-finance-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reefapi/refs/heads/main/openapi/reefapi-finance-data-api-openapi.yml
- filename: reefapi-government-tenders-api-openapi.yml
  format: yaml
  label: ReefAPI Government & Tenders API
  slug: reefapi-government-tenders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reefapi/refs/heads/main/openapi/reefapi-government-tenders-api-openapi.yml
- filename: reefapi-jobs-hiring-api-openapi.yml
  format: yaml
  label: ReefAPI Jobs & Hiring API
  slug: reefapi-jobs-hiring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reefapi/refs/heads/main/openapi/reefapi-jobs-hiring-api-openapi.yml
- filename: reefapi-media-film-knowledge-api-openapi.yml
  format: yaml
  label: ReefAPI Media, Film & Knowledge API
  slug: reefapi-media-film-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reefapi/refs/heads/main/openapi/reefapi-media-film-knowledge-api-openapi.yml
- filename: reefapi-other-api-openapi.yml
  format: yaml
  label: ReefAPI Other API
  slug: reefapi-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reefapi/refs/heads/main/openapi/reefapi-other-api-openapi.yml
- filename: reefapi-real-estate-api-openapi.yml
  format: yaml
  label: ReefAPI Real Estate API
  slug: reefapi-real-estate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reefapi/refs/heads/main/openapi/reefapi-real-estate-api-openapi.yml
- filename: reefapi-reputation-reviews-api-openapi.yml
  format: yaml
  label: ReefAPI Reputation & Reviews API
  slug: reefapi-reputation-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reefapi/refs/heads/main/openapi/reefapi-reputation-reviews-api-openapi.yml
- filename: reefapi-search-seo-api-openapi.yml
  format: yaml
  label: ReefAPI Search & SEO API
  slug: reefapi-search-seo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reefapi/refs/heads/main/openapi/reefapi-search-seo-api-openapi.yml
- filename: reefapi-social-media-api-openapi.yml
  format: yaml
  label: ReefAPI Social Media API
  slug: reefapi-social-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reefapi/refs/heads/main/openapi/reefapi-social-media-api-openapi.yml
- filename: reefapi-travel-lodging-api-openapi.yml
  format: yaml
  label: ReefAPI Travel & Lodging API
  slug: reefapi-travel-lodging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reefapi/refs/heads/main/openapi/reefapi-travel-lodging-api-openapi.yml
- filename: reefapi-utilities-ai-api-openapi.yml
  format: yaml
  label: ReefAPI Utilities & AI API
  slug: reefapi-utilities-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reefapi/refs/heads/main/openapi/reefapi-utilities-ai-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: reefapi.com
  spf: true
hosts:
- cert_expires: Nov  3 01:42:48 2026 GMT
  host: reefapi.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 01:42:48 2026 GMT
  host: api.reefapi.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15552000
  hsts_note: 'Re-probed 2026-08-31. The automated pass recorded hsts null because GET https://api.reefapi.com/ returns 404 (the API is POST-only, path-scoped); the 404 response nevertheless carries ''strict-transport-security: max-age=15552000; includeSubDomains'', as does a POST to a real operation. HSTS is served.'
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Reefapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ReefAPI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ReefAPI
provider_slug: reefapi
slug: reefapi-domain-security
source_filename: reefapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reefapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 01:42:48 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.reefapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 01:42:48 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n  hsts_include_subdomains: true\n  hsts_note: >-\n    Re-probed 2026-08-31. The automated pass recorded hsts null because\n    GET https://api.reefapi.com/ returns 404 (the API is POST-only, path-scoped);\n    the 404 response nevertheless carries\n    'strict-transport-security: max-age=15552000; includeSubDomains',\n    as does a POST to a real operation. HSTS is served.\ndomains:\n- domain: reefapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reefapi/refs/heads/main/security/reefapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Web Data
- Data Aggregation
- Web Scraping
- SERP
- E-Commerce
- Social Media
- Real Estate
- Job
- Travel
- News
- Finance
- Reviews
- Company Intelligence
- MCP
- Agent-Native
- REST
- OpenAPI
- llms-txt
- API Catalog
- Free Tier
- Credit
- Gateways
---
