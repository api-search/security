---
api_specs:
- filename: lathe-live-access-api-openapi.yml
  format: yaml
  label: Lathe Access API
  slug: lathe-live-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lathe-live/openapi/lathe-live-access-api-openapi.yml
- filename: lathe-live-account-api-openapi.yml
  format: yaml
  label: Lathe Account API
  slug: lathe-live-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lathe-live/openapi/lathe-live-account-api-openapi.yml
- filename: lathe-live-actions-api-openapi.yml
  format: yaml
  label: Lathe Actions API
  slug: lathe-live-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lathe-live/openapi/lathe-live-actions-api-openapi.yml
- filename: lathe-live-analytics-api-openapi.yml
  format: yaml
  label: Lathe Analytics API
  slug: lathe-live-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lathe-live/openapi/lathe-live-analytics-api-openapi.yml
- filename: lathe-live-apps-api-openapi.yml
  format: yaml
  label: Lathe Apps API
  slug: lathe-live-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lathe-live/openapi/lathe-live-apps-api-openapi.yml
- filename: lathe-live-catalogue-api-openapi.yml
  format: yaml
  label: Lathe Catalogue API
  slug: lathe-live-catalogue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lathe-live/openapi/lathe-live-catalogue-api-openapi.yml
- filename: lathe-live-engines-api-openapi.yml
  format: yaml
  label: Lathe Engines API
  slug: lathe-live-engines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lathe-live/openapi/lathe-live-engines-api-openapi.yml
- filename: lathe-live-instances-api-openapi.yml
  format: yaml
  label: Lathe Instances API
  slug: lathe-live-instances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lathe-live/openapi/lathe-live-instances-api-openapi.yml
- filename: lathe-live-jobs-api-openapi.yml
  format: yaml
  label: Lathe Jobs API
  slug: lathe-live-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lathe-live/openapi/lathe-live-jobs-api-openapi.yml
- filename: lathe-live-webhooks-api-openapi.yml
  format: yaml
  label: Lathe Webhooks API
  slug: lathe-live-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lathe-live/openapi/lathe-live-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lathe.live
  spf: true
hosts:
- cert_expires: Feb  3 21:54:44 2027 GMT
  host: lathe.live
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lathe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lathe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lathe
provider_slug: lathe-live
slug: lathe-live-domain-security
source_filename: lathe-live-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lathe.live\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 21:54:44 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lathe.live\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/lathe-live/security/lathe-live-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authentication
- PostgreSQL
- Redis
- NATS
- SeaweedFS
- Application
- Dedicated machine
- Flat-rate Pricing
---
