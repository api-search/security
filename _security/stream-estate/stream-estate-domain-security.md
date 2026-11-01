---
api_specs:
- filename: stream-estate-indicators-api-openapi.yml
  format: yaml
  label: stream-estate Indicators API
  slug: stream-estate-indicators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stream-estate/openapi/stream-estate-indicators-api-openapi.yml
- filename: stream-estate-properties-api-openapi.yml
  format: yaml
  label: stream-estate Properties API
  slug: stream-estate-properties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stream-estate/openapi/stream-estate-properties-api-openapi.yml
- filename: stream-estate-searches-api-openapi.yml
  format: yaml
  label: stream-estate Searches API
  slug: stream-estate-searches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stream-estate/openapi/stream-estate-searches-api-openapi.yml
- filename: stream-estate-webhooks-api-openapi.yml
  format: yaml
  label: stream-estate Webhooks API
  slug: stream-estate-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stream-estate/openapi/stream-estate-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: stream.estate
  spf: true
hosts:
- cert_expires: Dec  7 06:03:25 2026 GMT
  host: stream.estate
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Stream Estate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for stream-estate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: stream-estate
provider_slug: stream-estate
slug: stream-estate-domain-security
source_filename: stream-estate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stream.estate\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 06:03:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: stream.estate\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/stream-estate/security/stream-estate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- RealEstate
- PropTech
- DataAPI
- MarketAnalytics
- Valuation
---
