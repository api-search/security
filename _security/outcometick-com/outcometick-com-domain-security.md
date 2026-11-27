---
api_specs:
- filename: outcometick-com-backtest-api-openapi.yml
  format: yaml
  label: Outcometick Backtest API
  slug: outcometick-com-backtest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outcometick-com/openapi/outcometick-com-backtest-api-openapi.yml
- filename: outcometick-com-data-api-openapi.yml
  format: yaml
  label: Outcometick Data API
  slug: outcometick-com-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outcometick-com/openapi/outcometick-com-data-api-openapi.yml
- filename: outcometick-com-public-api-openapi.yml
  format: yaml
  label: Outcometick Public API
  slug: outcometick-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outcometick-com/openapi/outcometick-com-public-api-openapi.yml
- filename: outcometick-com-purchase-api-openapi.yml
  format: yaml
  label: Outcometick Purchase API
  slug: outcometick-com-purchase-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outcometick-com/openapi/outcometick-com-purchase-api-openapi.yml
- filename: outcometick-com-smart-money-api-openapi.yml
  format: yaml
  label: Outcometick Smart Money API
  slug: outcometick-com-smart-money-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outcometick-com/openapi/outcometick-com-smart-money-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: outcometick.com
  spf: true
hosts:
- cert_expires: Jan 12 04:31:06 2027 GMT
  host: outcometick.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Outcometick Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Outcometick, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Outcometick
provider_slug: outcometick-com
slug: outcometick-com-domain-security
source_filename: outcometick-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: outcometick.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 04:31:06 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: outcometick.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/outcometick-com/security/outcometick-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data
- Finance
- Cryptocurrency
- Market Data
---
