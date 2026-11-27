---
api_specs:
- filename: tripgain-com-aggregate-api-openapi.yml
  format: yaml
  label: TripGain Aggregate API
  slug: tripgain-com-aggregate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tripgain-com/openapi/tripgain-com-aggregate-api-openapi.yml
- filename: tripgain-com-analytics-api-openapi.yml
  format: yaml
  label: TripGain Analytics API
  slug: tripgain-com-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tripgain-com/openapi/tripgain-com-analytics-api-openapi.yml
- filename: tripgain-com-auth-api-openapi.yml
  format: yaml
  label: TripGain Auth API
  slug: tripgain-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tripgain-com/openapi/tripgain-com-auth-api-openapi.yml
- filename: tripgain-com-config-api-openapi.yml
  format: yaml
  label: TripGain Config API
  slug: tripgain-com-config-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tripgain-com/openapi/tripgain-com-config-api-openapi.yml
- filename: tripgain-com-flight-analytics-api-api-openapi.yml
  format: yaml
  label: TripGain Flight Analytics API
  slug: tripgain-com-flight-analytics-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tripgain-com/openapi/tripgain-com-flight-analytics-api-api-openapi.yml
- filename: tripgain-com-flight-search-api-openapi.yml
  format: yaml
  label: TripGain Flight Search API
  slug: tripgain-com-flight-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tripgain-com/openapi/tripgain-com-flight-search-api-openapi.yml
- filename: tripgain-com-gateway-request-analytics-api-openapi.yml
  format: yaml
  label: TripGain Gateway Request Analytics API
  slug: tripgain-com-gateway-request-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tripgain-com/openapi/tripgain-com-gateway-request-analytics-api-openapi.yml
- filename: tripgain-com-gateway-response-analytics-api-openapi.yml
  format: yaml
  label: TripGain Gateway Response Analytics API
  slug: tripgain-com-gateway-response-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tripgain-com/openapi/tripgain-com-gateway-response-analytics-api-openapi.yml
- filename: tripgain-com-gatewaylog-api-openapi.yml
  format: yaml
  label: TripGain Gateway Log API
  slug: tripgain-com-gatewaylog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tripgain-com/openapi/tripgain-com-gatewaylog-api-openapi.yml
- filename: tripgain-com-hotel-search-api-openapi.yml
  format: yaml
  label: TripGain Hotel Search API
  slug: tripgain-com-hotel-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tripgain-com/openapi/tripgain-com-hotel-search-api-openapi.yml
- filename: tripgain-com-ingest-batch-api-openapi.yml
  format: yaml
  label: TripGain Ingest Batch API
  slug: tripgain-com-ingest-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tripgain-com/openapi/tripgain-com-ingest-batch-api-openapi.yml
- filename: tripgain-com-ingest-hotel-batch-api-openapi.yml
  format: yaml
  label: TripGain Ingest Hotel Batch API
  slug: tripgain-com-ingest-hotel-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tripgain-com/openapi/tripgain-com-ingest-hotel-batch-api-openapi.yml
- filename: tripgain-com-ingest-hotel-single-api-openapi.yml
  format: yaml
  label: TripGain Ingest Hotel Single API
  slug: tripgain-com-ingest-hotel-single-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tripgain-com/openapi/tripgain-com-ingest-hotel-single-api-openapi.yml
- filename: tripgain-com-ingest-single-api-openapi.yml
  format: yaml
  label: TripGain Ingest Single API
  slug: tripgain-com-ingest-single-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tripgain-com/openapi/tripgain-com-ingest-single-api-openapi.yml
- filename: tripgain-com-stats-api-openapi.yml
  format: yaml
  label: TripGain Stats API
  slug: tripgain-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tripgain-com/openapi/tripgain-com-stats-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dns_aid:
    checked: '2026-11-27'
    published: false
  dnssec: false
  domain: tripgain.com
  spf: true
hosts:
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: tripgain.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: TripGain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TripGain, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TripGain
provider_slug: tripgain-com
slug: tripgain-com-domain-security
source_filename: tripgain-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tripgain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: tripgain.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dns_aid:\n    checked: '2026-11-27'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/tripgain-com/security/tripgain-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Travel
- AI
- Corporate
- ExpenseManagement
- Software
---
