---
api_specs:
- filename: green-screens-ai-analytics-api-openapi.yml
  format: yaml
  label: Green Screens AI Analytics API
  slug: green-screens-ai-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-screens-ai/refs/heads/main/openapi/green-screens-ai-analytics-api-openapi.yml
- filename: green-screens-ai-auth-api-openapi.yml
  format: yaml
  label: Green Screens AI Auth API
  slug: green-screens-ai-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-screens-ai/refs/heads/main/openapi/green-screens-ai-auth-api-openapi.yml
- filename: green-screens-ai-bids-api-openapi.yml
  format: yaml
  label: Green Screens AI Bids API
  slug: green-screens-ai-bids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-screens-ai/refs/heads/main/openapi/green-screens-ai-bids-api-openapi.yml
- filename: green-screens-ai-history-api-openapi.yml
  format: yaml
  label: Green Screens AI History API
  slug: green-screens-ai-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-screens-ai/refs/heads/main/openapi/green-screens-ai-history-api-openapi.yml
- filename: green-screens-ai-marketintelligence-api-openapi.yml
  format: yaml
  label: Green Screens AI MarketIntelligence API
  slug: green-screens-ai-marketintelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-screens-ai/refs/heads/main/openapi/green-screens-ai-marketintelligence-api-openapi.yml
- filename: green-screens-ai-prediction-api-openapi.yml
  format: yaml
  label: Green Screens AI Prediction API
  slug: green-screens-ai-prediction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-screens-ai/refs/heads/main/openapi/green-screens-ai-prediction-api-openapi.yml
- filename: green-screens-ai-pricing-api-openapi.yml
  format: yaml
  label: Green Screens AI Pricing API
  slug: green-screens-ai-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-screens-ai/refs/heads/main/openapi/green-screens-ai-pricing-api-openapi.yml
- filename: green-screens-ai-quotes-api-openapi.yml
  format: yaml
  label: Green Screens AI Quotes API
  slug: green-screens-ai-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-screens-ai/refs/heads/main/openapi/green-screens-ai-quotes-api-openapi.yml
- filename: green-screens-ai-tms-api-openapi.yml
  format: yaml
  label: Green Screens AI TMS API
  slug: green-screens-ai-tms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-screens-ai/refs/heads/main/openapi/green-screens-ai-tms-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: greenscreens.ai
  spf: true
hosts:
- host: www.greenscreens.ai
  https: false
- cert_expires: Mar 11 23:59:59 2027 GMT
  host: connect.greenscreens.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Green Screens Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Green Screens AI, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Green Screens AI
provider_slug: green-screens-ai
slug: green-screens-ai-domain-security
source_filename: green-screens-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.greenscreens.ai\n  https: false\n- host: connect.greenscreens.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: greenscreens.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/green-screens-ai/refs/heads/main/security/green-screens-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Freight
- Logistics
- Machine-Learning
- Pricing
- Transportation
---
