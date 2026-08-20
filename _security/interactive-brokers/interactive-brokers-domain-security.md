---
api_specs:
- filename: interactive-brokers-accounts-api-openapi.yml
  format: yaml
  label: Interactive Brokers Accounts API
  slug: interactive-brokers-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interactive-brokers/refs/heads/main/openapi/interactive-brokers-accounts-api-openapi.yml
- filename: interactive-brokers-contracts-api-openapi.yml
  format: yaml
  label: Interactive Brokers Contracts API
  slug: interactive-brokers-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interactive-brokers/refs/heads/main/openapi/interactive-brokers-contracts-api-openapi.yml
- filename: interactive-brokers-market-data-api-openapi.yml
  format: yaml
  label: Interactive Brokers Market Data API
  slug: interactive-brokers-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interactive-brokers/refs/heads/main/openapi/interactive-brokers-market-data-api-openapi.yml
- filename: interactive-brokers-orders-api-openapi.yml
  format: yaml
  label: Interactive Brokers Orders API
  slug: interactive-brokers-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interactive-brokers/refs/heads/main/openapi/interactive-brokers-orders-api-openapi.yml
- filename: interactive-brokers-portfolio-api-openapi.yml
  format: yaml
  label: Interactive Brokers Portfolio API
  slug: interactive-brokers-portfolio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interactive-brokers/refs/heads/main/openapi/interactive-brokers-portfolio-api-openapi.yml
- filename: interactive-brokers-sessions-api-openapi.yml
  format: yaml
  label: Interactive Brokers Sessions API
  slug: interactive-brokers-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interactive-brokers/refs/heads/main/openapi/interactive-brokers-sessions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: interactivebrokers.com
  spf: true
hosts:
- cert_expires: Aug  4 23:59:59 2026 GMT
  host: www.interactivebrokers.com
  hsts: true
  hsts_max_age: 600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Interactive Brokers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Interactive Brokers, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Interactive Brokers
provider_slug: interactive-brokers
slug: interactive-brokers-domain-security
source_filename: interactive-brokers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.interactivebrokers.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 600\ndomains:\n- domain: interactivebrokers.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/interactive-brokers/refs/heads/main/security/interactive-brokers-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Brokerage
- Market Data
- Order
- Portfolio
- Trading
---
