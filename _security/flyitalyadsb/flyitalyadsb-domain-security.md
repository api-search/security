---
api_specs:
- filename: flyitalyadsb-live-api-openapi.yml
  format: yaml
  label: FlyItalyADSB Live API
  slug: flyitalyadsb-live-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flyitalyadsb/openapi/flyitalyadsb-live-api-openapi.yml
- filename: flyitalyadsb-account-api-openapi.yml
  format: yaml
  label: FlyItalyADSB Account API
  slug: flyitalyadsb-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flyitalyadsb/openapi/flyitalyadsb-account-api-openapi.yml
- filename: flyitalyadsb-events-api-openapi.yml
  format: yaml
  label: FlyItalyADSB Events API
  slug: flyitalyadsb-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flyitalyadsb/openapi/flyitalyadsb-events-api-openapi.yml
- filename: flyitalyadsb-flights-api-openapi.yml
  format: yaml
  label: FlyItalyADSB Flights API
  slug: flyitalyadsb-flights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flyitalyadsb/openapi/flyitalyadsb-flights-api-openapi.yml
- filename: flyitalyadsb-history-api-openapi.yml
  format: yaml
  label: FlyItalyADSB History API
  slug: flyitalyadsb-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flyitalyadsb/openapi/flyitalyadsb-history-api-openapi.yml
- filename: flyitalyadsb-keys-api-openapi.yml
  format: yaml
  label: FlyItalyADSB Keys API
  slug: flyitalyadsb-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flyitalyadsb/openapi/flyitalyadsb-keys-api-openapi.yml
- filename: flyitalyadsb-live-api-openapi.yml
  format: yaml
  label: FlyItalyADSB Live API
  slug: flyitalyadsb-live-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flyitalyadsb/openapi/flyitalyadsb-live-api-openapi.yml
- filename: flyitalyadsb-watch-api-openapi.yml
  format: yaml
  label: FlyItalyADSB Watch API
  slug: flyitalyadsb-watch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flyitalyadsb/openapi/flyitalyadsb-watch-api-openapi.yml
- filename: flyitalyadsb-webhooks-api-openapi.yml
  format: yaml
  label: FlyItalyADSB Webhooks API
  slug: flyitalyadsb-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flyitalyadsb/openapi/flyitalyadsb-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: flyitalyadsb.com
  spf: true
hosts:
- cert_expires: Jan  9 22:40:53 2027 GMT
  host: flyitalyadsb.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 10 01:11:52 2027 GMT
  host: api.flyitalyadsb.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: FlyItalyADSB Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FlyItalyADSB, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: FlyItalyADSB
provider_slug: flyitalyadsb
slug: flyitalyadsb-domain-security
source_filename: flyitalyadsb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flyitalyadsb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 22:40:53 2027 GMT\n  hsts: false\n- host: api.flyitalyadsb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 01:11:52 2027 GMT\n  hsts: null\ndomains:\n- domain: flyitalyadsb.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/flyitalyadsb/security/flyitalyadsb-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- ADS-B
- MLAT
- Aviation
- Flight Tracking
- Open Data
---
