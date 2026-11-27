---
api_specs:
- filename: earningsfeed-com-account-api-openapi.yml
  format: yaml
  label: Earnings Feed Account API
  slug: earningsfeed-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/earningsfeed-com/openapi/earningsfeed-com-account-api-openapi.yml
- filename: earningsfeed-com-companies-api-openapi.yml
  format: yaml
  label: Earnings Feed Companies API
  slug: earningsfeed-com-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/earningsfeed-com/openapi/earningsfeed-com-companies-api-openapi.yml
- filename: earningsfeed-com-filings-api-openapi.yml
  format: yaml
  label: Earnings Feed Filings API
  slug: earningsfeed-com-filings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/earningsfeed-com/openapi/earningsfeed-com-filings-api-openapi.yml
- filename: earningsfeed-com-insider-api-openapi.yml
  format: yaml
  label: Earnings Feed Insider API
  slug: earningsfeed-com-insider-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/earningsfeed-com/openapi/earningsfeed-com-insider-api-openapi.yml
- filename: earningsfeed-com-institutional-api-openapi.yml
  format: yaml
  label: Earnings Feed Institutional API
  slug: earningsfeed-com-institutional-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/earningsfeed-com/openapi/earningsfeed-com-institutional-api-openapi.yml
- filename: earningsfeed-com-webhooks-api-openapi.yml
  format: yaml
  label: Earnings Feed Webhooks API
  slug: earningsfeed-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/earningsfeed-com/openapi/earningsfeed-com-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: earningsfeed.com
  spf: true
hosts:
- cert_expires: Jan 10 05:31:18 2027 GMT
  host: earningsfeed.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Earnings Feed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Earnings Feed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Earnings Feed
provider_slug: earningsfeed-com
slug: earningsfeed-com-domain-security
source_filename: earningsfeed-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: earningsfeed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 05:31:18 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: earningsfeed.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/earningsfeed-com/security/earningsfeed-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- SEC
- Filings
- Data
---
