---
api_specs:
- filename: bolsai-admin-api-openapi.yml
  format: yaml
  label: Bolsai Admin API
  slug: bolsai-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolsai/refs/heads/main/openapi/bolsai-admin-api-openapi.yml
- filename: bolsai-api-keys-api-openapi.yml
  format: yaml
  label: Bolsai API Keys API
  slug: bolsai-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolsai/refs/heads/main/openapi/bolsai-api-keys-api-openapi.yml
- filename: bolsai-auth-api-openapi.yml
  format: yaml
  label: Bolsai Auth API
  slug: bolsai-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolsai/refs/heads/main/openapi/bolsai-auth-api-openapi.yml
- filename: bolsai-billing-api-openapi.yml
  format: yaml
  label: Bolsai Billing API
  slug: bolsai-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolsai/refs/heads/main/openapi/bolsai-billing-api-openapi.yml
- filename: bolsai-companies-api-openapi.yml
  format: yaml
  label: Bolsai Companies API
  slug: bolsai-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolsai/refs/heads/main/openapi/bolsai-companies-api-openapi.yml
- filename: bolsai-dividends-api-openapi.yml
  format: yaml
  label: Bolsai Dividends API
  slug: bolsai-dividends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolsai/refs/heads/main/openapi/bolsai-dividends-api-openapi.yml
- filename: bolsai-feedback-api-openapi.yml
  format: yaml
  label: Bolsai Feedback API
  slug: bolsai-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolsai/refs/heads/main/openapi/bolsai-feedback-api-openapi.yml
- filename: bolsai-fiis-api-openapi.yml
  format: yaml
  label: Bolsai Fiis API
  slug: bolsai-fiis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolsai/refs/heads/main/openapi/bolsai-fiis-api-openapi.yml
- filename: bolsai-financials-api-openapi.yml
  format: yaml
  label: Bolsai Financials API
  slug: bolsai-financials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolsai/refs/heads/main/openapi/bolsai-financials-api-openapi.yml
- filename: bolsai-fundamentals-api-openapi.yml
  format: yaml
  label: Bolsai Fundamentals API
  slug: bolsai-fundamentals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolsai/refs/heads/main/openapi/bolsai-fundamentals-api-openapi.yml
- filename: bolsai-health-api-openapi.yml
  format: yaml
  label: Bolsai Health API
  slug: bolsai-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolsai/refs/heads/main/openapi/bolsai-health-api-openapi.yml
- filename: bolsai-macro-api-openapi.yml
  format: yaml
  label: Bolsai Macro API
  slug: bolsai-macro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolsai/refs/heads/main/openapi/bolsai-macro-api-openapi.yml
- filename: bolsai-screener-api-openapi.yml
  format: yaml
  label: Bolsai Screener API
  slug: bolsai-screener-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolsai/refs/heads/main/openapi/bolsai-screener-api-openapi.yml
- filename: bolsai-stocks-api-openapi.yml
  format: yaml
  label: Bolsai Stocks API
  slug: bolsai-stocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolsai/refs/heads/main/openapi/bolsai-stocks-api-openapi.yml
- filename: bolsai-oauth-api-openapi.yml
  format: yaml
  label: Bolsai OAUTH API
  slug: bolsai-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolsai/refs/heads/main/openapi/bolsai-oauth-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: usebolsai.com
  spf: true
hosts:
- cert_expires: Oct 18 15:25:29 2026 GMT
  host: usebolsai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 15:25:29 2026 GMT
  host: api.usebolsai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Bolsai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bolsai, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bolsai
provider_slug: bolsai
slug: bolsai-domain-security
source_filename: bolsai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usebolsai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 15:25:29 2026 GMT\n  hsts: false\n- host: api.usebolsai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 15:25:29 2026 GMT\n  hsts: false\ndomains:\n- domain: usebolsai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bolsai/refs/heads/main/security/bolsai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Finance
- Financial Data
- Market Data
- Stocks/equities
- Real Estate Funds
- Dividends
- Fundamentals
- Macroeconomic Data
- Brazil
- Developer Tools
- MCP
- AI Agents
---
