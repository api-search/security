---
api_specs:
- filename: scrunch-ai-agent-traffic-api-openapi.yml
  format: yaml
  label: Scrunch AI agent-traffic API
  slug: scrunch-ai-agent-traffic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrunch-ai/refs/heads/main/openapi/scrunch-ai-agent-traffic-api-openapi.yml
- filename: scrunch-ai-ai-referrals-api-openapi.yml
  format: yaml
  label: Scrunch AI ai-referrals API
  slug: scrunch-ai-ai-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrunch-ai/refs/heads/main/openapi/scrunch-ai-ai-referrals-api-openapi.yml
- filename: scrunch-ai-axp-render-api-openapi.yml
  format: yaml
  label: Scrunch AI axp-render API
  slug: scrunch-ai-axp-render-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrunch-ai/refs/heads/main/openapi/scrunch-ai-axp-render-api-openapi.yml
- filename: scrunch-ai-brands-api-openapi.yml
  format: yaml
  label: Scrunch AI Brands API
  slug: scrunch-ai-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrunch-ai/refs/heads/main/openapi/scrunch-ai-brands-api-openapi.yml
- filename: scrunch-ai-orchestration-api-openapi.yml
  format: yaml
  label: Scrunch AI orchestration API
  slug: scrunch-ai-orchestration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrunch-ai/refs/heads/main/openapi/scrunch-ai-orchestration-api-openapi.yml
- filename: scrunch-ai-page-audits-api-openapi.yml
  format: yaml
  label: Scrunch AI Page Audits API
  slug: scrunch-ai-page-audits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrunch-ai/refs/heads/main/openapi/scrunch-ai-page-audits-api-openapi.yml
- filename: scrunch-ai-prompts-api-openapi.yml
  format: yaml
  label: Scrunch AI Prompts API
  slug: scrunch-ai-prompts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrunch-ai/refs/heads/main/openapi/scrunch-ai-prompts-api-openapi.yml
- filename: scrunch-ai-query-api-openapi.yml
  format: yaml
  label: Scrunch AI Query API
  slug: scrunch-ai-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrunch-ai/refs/heads/main/openapi/scrunch-ai-query-api-openapi.yml
- filename: scrunch-ai-responses-api-openapi.yml
  format: yaml
  label: Scrunch AI Responses API
  slug: scrunch-ai-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrunch-ai/refs/heads/main/openapi/scrunch-ai-responses-api-openapi.yml
- filename: scrunch-ai-sitemap-api-openapi.yml
  format: yaml
  label: Scrunch AI sitemap API
  slug: scrunch-ai-sitemap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrunch-ai/refs/heads/main/openapi/scrunch-ai-sitemap-api-openapi.yml
- filename: scrunch-ai-signals-api-openapi.yml
  format: yaml
  label: Scrunch AI Signals API
  slug: scrunch-ai-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrunch-ai/refs/heads/main/openapi/scrunch-ai-signals-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: scrunch.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: scrunchai.com
  spf: true
hosts:
- cert_expires: Oct 16 08:53:44 2026 GMT
  host: scrunch.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 09:21:45 2026 GMT
  host: developers.scrunch.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 11:44:10 2026 GMT
  host: api.scrunchai.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scrunch Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scrunch AI, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Scrunch AI
provider_slug: scrunch-ai
slug: scrunch-ai-domain-security
source_filename: scrunch-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scrunch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 08:53:44 2026 GMT\n  hsts: false\n- host: developers.scrunch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 09:21:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.scrunchai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 11:44:10 2026 GMT\n  hsts: null\ndomains:\n- domain: scrunch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: scrunchai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scrunch-ai/refs/heads/main/security/scrunch-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- AI Search
- Answer Engine Optimization
- Generative Engine Optimization
- Brand Visibility
- Analytics
- SEO
- Agent Experience
- MCP
---
