---
api_specs:
- filename: fed-spend-com-contracts-api-openapi.yml
  format: yaml
  label: Fed-Spend Contracts API
  slug: fed-spend-com-contracts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fed-spend-com/openapi/fed-spend-com-contracts-api-openapi.yml
- filename: fed-spend-com-search-api-openapi.yml
  format: yaml
  label: Fed-Spend Search API
  slug: fed-spend-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fed-spend-com/openapi/fed-spend-com-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fed-spend.com
  spf: true
hosts:
- cert_expires: Dec 19 07:49:21 2026 GMT
  host: fed-spend.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fed-Spend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fed-Spend, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Fed-Spend
provider_slug: fed-spend-com
slug: fed-spend-com-domain-security
source_filename: fed-spend-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fed-spend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 07:49:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fed-spend.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/fed-spend-com/security/fed-spend-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Business Intelligence
- Government
- Federal Spending
- Data Analytics
- Contract Intelligence
- Company
---
