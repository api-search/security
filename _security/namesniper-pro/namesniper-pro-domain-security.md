---
api_specs:
- filename: namesniper-pro-account-api-openapi.yml
  format: yaml
  label: NameSniper Account API
  slug: namesniper-pro-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namesniper-pro/openapi/namesniper-pro-account-api-openapi.yml
- filename: namesniper-pro-check-api-openapi.yml
  format: yaml
  label: NameSniper Check API
  slug: namesniper-pro-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namesniper-pro/openapi/namesniper-pro-check-api-openapi.yml
- filename: namesniper-pro-generate-api-openapi.yml
  format: yaml
  label: NameSniper Generate API
  slug: namesniper-pro-generate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namesniper-pro/openapi/namesniper-pro-generate-api-openapi.yml
- filename: namesniper-pro-monitoring-api-openapi.yml
  format: yaml
  label: NameSniper Monitoring API
  slug: namesniper-pro-monitoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namesniper-pro/openapi/namesniper-pro-monitoring-api-openapi.yml
- filename: namesniper-pro-trademark-api-openapi.yml
  format: yaml
  label: NameSniper Trademark API
  slug: namesniper-pro-trademark-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namesniper-pro/openapi/namesniper-pro-trademark-api-openapi.yml
- filename: namesniper-pro-webhooks-api-openapi.yml
  format: yaml
  label: NameSniper Webhooks API
  slug: namesniper-pro-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namesniper-pro/openapi/namesniper-pro-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: namesniper.pro
  spf: true
hosts:
- cert_expires: Jan  5 08:50:19 2027 GMT
  host: namesniper.pro
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: NameSniper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NameSniper, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: NameSniper
provider_slug: namesniper-pro
slug: namesniper-pro-domain-security
source_filename: namesniper-pro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: namesniper.pro\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 08:50:19 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: namesniper.pro\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/namesniper-pro/security/namesniper-pro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- UsernameChecker
- HandleMonitor
- Social Media
- Domain Search
---
