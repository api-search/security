---
api_specs:
- filename: maddog-finance-access-api-openapi.yml
  format: yaml
  label: MADDOG Access API
  slug: maddog-finance-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maddog-finance/openapi/maddog-finance-access-api-openapi.yml
- filename: maddog-finance-backtesting-api-openapi.yml
  format: yaml
  label: MADDOG Backtesting API
  slug: maddog-finance-backtesting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maddog-finance/openapi/maddog-finance-backtesting-api-openapi.yml
- filename: maddog-finance-market-data-api-openapi.yml
  format: yaml
  label: MADDOG Market data API
  slug: maddog-finance-market-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maddog-finance/openapi/maddog-finance-market-data-api-openapi.yml
- filename: maddog-finance-market-statistics-api-openapi.yml
  format: yaml
  label: MADDOG Market statistics API
  slug: maddog-finance-market-statistics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maddog-finance/openapi/maddog-finance-market-statistics-api-openapi.yml
- filename: maddog-finance-service-api-openapi.yml
  format: yaml
  label: MADDOG Service API
  slug: maddog-finance-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maddog-finance/openapi/maddog-finance-service-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: maddog.finance
  spf: false
hosts:
- cert_expires: Jan 11 19:04:55 2027 GMT
  host: maddog.finance
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MADDOG Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MADDOG, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: MADDOG
provider_slug: maddog-finance
slug: maddog-finance-domain-security
source_filename: maddog-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: maddog.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 19:04:55 2027 GMT\n  hsts: false\ndomains:\n- domain: maddog.finance\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/maddog-finance/security/maddog-finance-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Trading
- Finance
- Analytics
- Price-Action
---
