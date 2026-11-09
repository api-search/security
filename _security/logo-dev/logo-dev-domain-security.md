---
api_specs:
- filename: logo-dev-account-api-openapi.yml
  format: yaml
  label: Logo.dev Account API
  slug: logo-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logo-dev/openapi/logo-dev-account-api-openapi.yml
- filename: logo-dev-brands-api-openapi.yml
  format: yaml
  label: Logo.dev Brands API
  slug: logo-dev-brands-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logo-dev/openapi/logo-dev-brands-api-openapi.yml
- filename: logo-dev-flags-api-openapi.yml
  format: yaml
  label: Logo.dev Flags API
  slug: logo-dev-flags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logo-dev/openapi/logo-dev-flags-api-openapi.yml
- filename: logo-dev-logo-cdn-api-openapi.yml
  format: yaml
  label: Logo.dev Logo CDN API
  slug: logo-dev-logo-cdn-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logo-dev/openapi/logo-dev-logo-cdn-api-openapi.yml
- filename: logo-dev-logos-api-openapi.yml
  format: yaml
  label: Logo.dev Logos API
  slug: logo-dev-logos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logo-dev/openapi/logo-dev-logos-api-openapi.yml
- filename: logo-dev-search-api-openapi.yml
  format: yaml
  label: Logo.dev Search API
  slug: logo-dev-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logo-dev/openapi/logo-dev-search-api-openapi.yml
- filename: logo-dev-subscriptions-api-openapi.yml
  format: yaml
  label: Logo.dev Subscriptions API
  slug: logo-dev-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logo-dev/openapi/logo-dev-subscriptions-api-openapi.yml
- filename: logo-dev-transaction-enrichment-api-api-openapi.yml
  format: yaml
  label: Logo.dev Transaction Enrichment API
  slug: logo-dev-transaction-enrichment-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logo-dev/openapi/logo-dev-transaction-enrichment-api-api-openapi.yml
- filename: logo-dev-webhook-endpoints-api-openapi.yml
  format: yaml
  label: Logo.dev Webhook endpoints API
  slug: logo-dev-webhook-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logo-dev/openapi/logo-dev-webhook-endpoints-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: logo.dev
  spf: true
hosts:
- cert_expires: Jan 14 02:39:41 2027 GMT
  host: logo.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Logo Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Logo.dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Logo.dev
provider_slug: logo-dev
slug: logo-dev-domain-security
source_filename: logo-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: logo.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 02:39:41 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: logo.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/logo-dev/security/logo-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Logo
- Branding
- CDN
- Free Tier
---
