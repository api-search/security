---
api_specs:
- filename: morningstar-oauth-api-openapi.yml
  format: yaml
  label: Morningstar Authentication API
  slug: morningstar-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-oauth-api-openapi.yml
- filename: morningstar-corporate-actions-api-openapi.yml
  format: yaml
  label: Morningstar Time Series API
  slug: morningstar-time-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-corporate-actions-api-openapi.yml
- filename: morningstar-data-points-api-openapi.yml
  format: yaml
  label: Morningstar Screener APIs
  slug: morningstar-screener-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-data-points-api-openapi.yml
- filename: morningstar-aggregates-financials-api-openapi.yml
  format: yaml
  label: Morningstar Investment Details APIs
  slug: morningstar-investment-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-aggregates-financials-api-openapi.yml
- filename: morningstar-investment-list-api-openapi.yml
  format: yaml
  label: Morningstar Investment List API
  slug: morningstar-investment-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-investment-list-api-openapi.yml
- filename: morningstar-esg-api-openapi.yml
  format: yaml
  label: Morningstar Portfolio Analysis APIs
  slug: morningstar-portfolio-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-esg-api-openapi.yml
- filename: morningstar-analyst-highlights-api-openapi.yml
  format: yaml
  label: Morningstar AI Insights API
  slug: morningstar-ai-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-analyst-highlights-api-openapi.yml
- filename: morningstar-scenario-analysis-api-openapi.yml
  format: yaml
  label: Morningstar Scenario Analysis API
  slug: morningstar-scenario-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-scenario-analysis-api-openapi.yml
- filename: morningstar-clients-api-openapi.yml
  format: yaml
  label: Morningstar Risk Profiler API
  slug: morningstar-risk-profiler-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-clients-api-openapi.yml
- filename: morningstar-investments-universe-api-openapi.yml
  format: yaml
  label: Morningstar Universe API
  slug: morningstar-universe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-investments-universe-api-openapi.yml
- filename: morningstar-benchmarkfees-api-openapi.yml
  format: yaml
  label: Morningstar Financial Planning APIs
  slug: morningstar-financial-planning-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-benchmarkfees-api-openapi.yml
- filename: morningstar-attribution-api-openapi.yml
  format: yaml
  label: Morningstar Investment Analysis APIs
  slug: morningstar-investment-analysis-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-attribution-api-openapi.yml
- filename: morningstar-accounts-api-openapi.yml
  format: yaml
  label: Morningstar ByAllAccounts API
  slug: morningstar-byallaccounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-accounts-api-openapi.yml
- filename: morningstar-morningstar-agent-api-openapi.yml
  format: yaml
  label: Morningstar Agent API
  slug: morningstar-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-morningstar-agent-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: morningstar.com
  spf: true
hosts:
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: www.morningstar.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: developer.morningstar.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: www.us-api.morningstar.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Morningstar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Morningstar, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Morningstar
provider_slug: morningstar
slug: morningstar-domain-security
source_filename: morningstar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.morningstar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: false\n- host: developer.morningstar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.us-api.morningstar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: morningstar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/security/morningstar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial
- Market Data
- Investing
- Stocks
- Funds
- Real-Time
- Reference Data
- Portfolio Analytics
- Research
- Indexes
---
