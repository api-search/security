---
api_specs:
- filename: dataforseo-aioptimization-api-openapi.yml
  format: yaml
  label: DataForSEO AiOptimization API
  slug: dataforseo-aioptimization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/openapi/dataforseo-aioptimization-api-openapi.yml
- filename: dataforseo-appdata-api-openapi.yml
  format: yaml
  label: DataForSEO AppData API
  slug: dataforseo-appdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/openapi/dataforseo-appdata-api-openapi.yml
- filename: dataforseo-appendix-api-openapi.yml
  format: yaml
  label: DataForSEO Appendix API
  slug: dataforseo-appendix-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/openapi/dataforseo-appendix-api-openapi.yml
- filename: dataforseo-backlinks-api-openapi.yml
  format: yaml
  label: DataForSEO Backlinks API
  slug: dataforseo-backlinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/openapi/dataforseo-backlinks-api-openapi.yml
- filename: dataforseo-businessdata-api-openapi.yml
  format: yaml
  label: DataForSEO BusinessData API
  slug: dataforseo-businessdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/openapi/dataforseo-businessdata-api-openapi.yml
- filename: dataforseo-contentanalysis-api-openapi.yml
  format: yaml
  label: DataForSEO ContentAnalysis API
  slug: dataforseo-contentanalysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/openapi/dataforseo-contentanalysis-api-openapi.yml
- filename: dataforseo-dataforseolabs-api-openapi.yml
  format: yaml
  label: DataForSEO DataforseoLabs API
  slug: dataforseo-dataforseolabs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/openapi/dataforseo-dataforseolabs-api-openapi.yml
- filename: dataforseo-domainanalytics-api-openapi.yml
  format: yaml
  label: DataForSEO DomainAnalytics API
  slug: dataforseo-domainanalytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/openapi/dataforseo-domainanalytics-api-openapi.yml
- filename: dataforseo-keywordsdata-api-openapi.yml
  format: yaml
  label: DataForSEO KeywordsData API
  slug: dataforseo-keywordsdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/openapi/dataforseo-keywordsdata-api-openapi.yml
- filename: dataforseo-merchant-api-openapi.yml
  format: yaml
  label: DataForSEO Merchant API
  slug: dataforseo-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/openapi/dataforseo-merchant-api-openapi.yml
- filename: dataforseo-onpage-api-openapi.yml
  format: yaml
  label: DataForSEO OnPage API
  slug: dataforseo-onpage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/openapi/dataforseo-onpage-api-openapi.yml
- filename: dataforseo-serp-api-openapi.yml
  format: yaml
  label: DataForSEO Serp API
  slug: dataforseo-serp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/openapi/dataforseo-serp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dataforseo.com
  spf: true
hosts:
- cert_expires: Aug 20 23:33:08 2026 GMT
  host: dataforseo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 18 23:59:59 2027 GMT
  host: api.dataforseo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 18 23:59:59 2027 GMT
  host: sandbox.dataforseo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dataforseo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DataForSEO, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DataForSEO
provider_slug: dataforseo
slug: dataforseo-domain-security
source_filename: dataforseo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dataforseo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 23:33:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.dataforseo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 23:59:59 2027 GMT\n  hsts: null\n- host: sandbox.dataforseo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: dataforseo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/security/dataforseo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SEO
- SERP
- Keywords
- Backlinks
- Domain Analytics
- On-Page SEO
- Competitor Research
- Search Engines
- Content Analysis
- E-Commerce
- App Store
- Business Data
- AI Optimization
- Social-Media
---
