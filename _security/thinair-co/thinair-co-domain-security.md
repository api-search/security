---
api_specs:
- filename: thinair-co-account-api-openapi.yml
  format: yaml
  label: thinair-co Account API
  slug: thinair-co-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thinair-co/openapi/thinair-co-account-api-openapi.yml
- filename: thinair-co-billing-api-openapi.yml
  format: yaml
  label: thinair-co Billing API
  slug: thinair-co-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thinair-co/openapi/thinair-co-billing-api-openapi.yml
- filename: thinair-co-conditions-api-openapi.yml
  format: yaml
  label: thinair-co Conditions API
  slug: thinair-co-conditions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thinair-co/openapi/thinair-co-conditions-api-openapi.yml
- filename: thinair-co-connections-api-openapi.yml
  format: yaml
  label: thinair-co Connections API
  slug: thinair-co-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thinair-co/openapi/thinair-co-connections-api-openapi.yml
- filename: thinair-co-geocoding-api-openapi.yml
  format: yaml
  label: thinair-co Geocoding API
  slug: thinair-co-geocoding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thinair-co/openapi/thinair-co-geocoding-api-openapi.yml
- filename: thinair-co-geofences-api-openapi.yml
  format: yaml
  label: thinair-co Geofences API
  slug: thinair-co-geofences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thinair-co/openapi/thinair-co-geofences-api-openapi.yml
- filename: thinair-co-intersections-api-openapi.yml
  format: yaml
  label: thinair-co Intersections API
  slug: thinair-co-intersections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thinair-co/openapi/thinair-co-intersections-api-openapi.yml
- filename: thinair-co-learning-api-openapi.yml
  format: yaml
  label: thinair-co Learning API
  slug: thinair-co-learning-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thinair-co/openapi/thinair-co-learning-api-openapi.yml
- filename: thinair-co-migrations-api-openapi.yml
  format: yaml
  label: thinair-co Migrations API
  slug: thinair-co-migrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thinair-co/openapi/thinair-co-migrations-api-openapi.yml
- filename: thinair-co-places-api-openapi.yml
  format: yaml
  label: thinair-co Places API
  slug: thinair-co-places-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thinair-co/openapi/thinair-co-places-api-openapi.yml
- filename: thinair-co-query-api-openapi.yml
  format: yaml
  label: thinair-co Query API
  slug: thinair-co-query-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thinair-co/openapi/thinair-co-query-api-openapi.yml
- filename: thinair-co-routing-api-openapi.yml
  format: yaml
  label: thinair-co Routing API
  slug: thinair-co-routing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thinair-co/openapi/thinair-co-routing-api-openapi.yml
- filename: thinair-co-tables-api-openapi.yml
  format: yaml
  label: thinair-co Tables API
  slug: thinair-co-tables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thinair-co/openapi/thinair-co-tables-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: thinair.co
  spf: true
hosts:
- cert_expires: Jan  8 06:25:51 2027 GMT
  host: thinair.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Thinair Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for thinair-co, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: thinair-co
provider_slug: thinair-co
slug: thinair-co-domain-security
source_filename: thinair-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thinair.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 06:25:51 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: thinair.co\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/thinair-co/security/thinair-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- fleet-management
- telematics
- logistics
- compliance
- API
---
