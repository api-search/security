---
api_specs:
- filename: overview
  format: yaml
  label: SE Ranking Data API
  slug: data-api
  spec_type: Postman
  url: https://www.postman.com/serankingdev/se-ranking-developers/overview
- filename: overview
  format: yaml
  label: SE Ranking Project API
  slug: project-api
  spec_type: Postman
  url: https://www.postman.com/serankingdev/se-ranking-developers/overview
- filename: se-ranking-account-system-api-openapi.yml
  format: yaml
  label: SE Ranking Account & system API
  slug: se-ranking-account-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/se-ranking/refs/heads/main/openapi/se-ranking-account-system-api-openapi.yml
- filename: se-ranking-ai-search-api-openapi.yml
  format: yaml
  label: SE Ranking AI search API
  slug: se-ranking-ai-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/se-ranking/refs/heads/main/openapi/se-ranking-ai-search-api-openapi.yml
- filename: se-ranking-backlinks-api-openapi.yml
  format: yaml
  label: SE Ranking backlinks API
  slug: se-ranking-backlinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/se-ranking/refs/heads/main/openapi/se-ranking-backlinks-api-openapi.yml
- filename: se-ranking-domain-analysis-api-openapi.yml
  format: yaml
  label: SE Ranking Domain Analysis API
  slug: se-ranking-domain-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/se-ranking/refs/heads/main/openapi/se-ranking-domain-analysis-api-openapi.yml
- filename: se-ranking-keyword-research-api-openapi.yml
  format: yaml
  label: SE Ranking Keyword Research API
  slug: se-ranking-keyword-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/se-ranking/refs/heads/main/openapi/se-ranking-keyword-research-api-openapi.yml
- filename: se-ranking-serp-results-classic-api-openapi.yml
  format: yaml
  label: SE Ranking SERP Results > classic API
  slug: se-ranking-serp-results-classic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/se-ranking/refs/heads/main/openapi/se-ranking-serp-results-classic-api-openapi.yml
- filename: se-ranking-website-audit-api-openapi.yml
  format: yaml
  label: SE Ranking Website Audit API
  slug: se-ranking-website-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/se-ranking/refs/heads/main/openapi/se-ranking-website-audit-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: seranking.com
  spf: true
hosts:
- cert_expires: Oct 12 22:17:43 2026 GMT
  host: seranking.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 05:46:42 2026 GMT
  host: api.seranking.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Se Ranking Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SE Ranking, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SE Ranking
provider_slug: se-ranking
slug: se-ranking-domain-security
source_filename: se-ranking-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: seranking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 22:17:43 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: api.seranking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 05:46:42 2026 GMT\n  hsts: null\ndomains:\n- domain: seranking.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/se-ranking/refs/heads/main/security/se-ranking-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SEO
- Keyword Research
- Rank Tracking
- Backlinks
- Competitor Analysis
- Website Audit
- AI Search
- GEO
- Digital Marketing
- MCP
- AI Agents
- Agent Skills
---
