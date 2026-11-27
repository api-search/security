---
api_specs:
- filename: cpz-lab-com-accounts-api-openapi.yml
  format: yaml
  label: CPZ Lab Accounts API
  slug: cpz-lab-com-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-accounts-api-openapi.yml
- filename: cpz-lab-com-actions-api-openapi.yml
  format: yaml
  label: CPZ Lab Actions API
  slug: cpz-lab-com-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-actions-api-openapi.yml
- filename: cpz-lab-com-backtests-api-openapi.yml
  format: yaml
  label: CPZ Lab Backtests API
  slug: cpz-lab-com-backtests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-backtests-api-openapi.yml
- filename: cpz-lab-com-cash-api-openapi.yml
  format: yaml
  label: CPZ Lab Cash API
  slug: cpz-lab-com-cash-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-cash-api-openapi.yml
- filename: cpz-lab-com-data-files-api-openapi.yml
  format: yaml
  label: CPZ Lab Data Files API
  slug: cpz-lab-com-data-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-data-files-api-openapi.yml
- filename: cpz-lab-com-me-api-openapi.yml
  format: yaml
  label: CPZ Lab Me API
  slug: cpz-lab-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-me-api-openapi.yml
- filename: cpz-lab-com-order-approvals-api-openapi.yml
  format: yaml
  label: CPZ Lab Order Approvals API
  slug: cpz-lab-com-order-approvals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-order-approvals-api-openapi.yml
- filename: cpz-lab-com-orders-api-openapi.yml
  format: yaml
  label: CPZ Lab Orders API
  slug: cpz-lab-com-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-orders-api-openapi.yml
- filename: cpz-lab-com-positions-api-openapi.yml
  format: yaml
  label: CPZ Lab Positions API
  slug: cpz-lab-com-positions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-positions-api-openapi.yml
- filename: cpz-lab-com-risk-snapshots-api-openapi.yml
  format: yaml
  label: CPZ Lab Risk Snapshots API
  slug: cpz-lab-com-risk-snapshots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-risk-snapshots-api-openapi.yml
- filename: cpz-lab-com-strategies-api-openapi.yml
  format: yaml
  label: CPZ Lab Strategies API
  slug: cpz-lab-com-strategies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-strategies-api-openapi.yml
- filename: cpz-lab-com-transactions-api-openapi.yml
  format: yaml
  label: CPZ Lab Transactions API
  slug: cpz-lab-com-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-transactions-api-openapi.yml
- filename: cpz-lab-com-watchlist-api-openapi.yml
  format: yaml
  label: CPZ Lab Watchlist API
  slug: cpz-lab-com-watchlist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-watchlist-api-openapi.yml
- filename: cpz-lab-com-webhooks-api-openapi.yml
  format: yaml
  label: CPZ Lab Webhooks API
  slug: cpz-lab-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cpz-lab-com/openapi/cpz-lab-com-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cpz-lab.com
  spf: true
hosts:
- cert_expires: Jan  5 05:15:02 2027 GMT
  host: cpz-lab.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 27 19:28:20 2027 GMT
  host: ai.cpz-lab.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 22:32:37 2027 GMT
  host: api.cpz-lab.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: CPZ Lab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CPZ Lab, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CPZ Lab
provider_slug: cpz-lab-com
slug: cpz-lab-com-domain-security
source_filename: cpz-lab-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cpz-lab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 05:15:02 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: ai.cpz-lab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 19:28:20 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.cpz-lab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 22:32:37 2027 GMT\n  hsts: null\ndomains:\n- domain: cpz-lab.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cpz-lab-com/security/cpz-lab-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Trading
- Algorithmic Trading
- Quantitative Finance
- Backtesting
- Risk Management
- Artificial Intelligence
- MCP
- Python SDK
---
