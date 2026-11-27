---
api_specs:
- filename: mukoko-com-news-api-openapi.yml
  format: yaml
  label: Mukoko News API
  slug: mukoko-com-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mukoko-com/openapi/mukoko-com-news-api-openapi.yml
- filename: mukoko-com-service-api-openapi.yml
  format: yaml
  label: Mukoko Service API
  slug: mukoko-com-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mukoko-com/openapi/mukoko-com-service-api-openapi.yml
- filename: mukoko-com-weather-api-openapi.yml
  format: yaml
  label: Mukoko Weather API
  slug: mukoko-com-weather-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mukoko-com/openapi/mukoko-com-weather-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: mukoko.com
  spf: true
hosts:
- cert_expires: Feb  5 04:06:51 2027 GMT
  host: mukoko.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mukoko Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mukoko, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Mukoko
provider_slug: mukoko-com
slug: mukoko-com-domain-security
source_filename: mukoko-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mukoko.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 04:06:51 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mukoko.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mukoko-com/security/mukoko-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Super App
- Africa
- Event
- Weather
- News
---
