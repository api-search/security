---
api_specs:
- filename: openwaters-io-authentication-api-openapi.yml
  format: yaml
  label: Open Waters Authentication API
  slug: openwaters-io-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openwaters-io/openapi/openwaters-io-authentication-api-openapi.yml
- filename: openwaters-io-contributing-api-openapi.yml
  format: yaml
  label: Open Waters Contributing API
  slug: openwaters-io-contributing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openwaters-io/openapi/openwaters-io-contributing-api-openapi.yml
- filename: openwaters-io-currents-api-openapi.yml
  format: yaml
  label: Open Waters Currents API
  slug: openwaters-io-currents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openwaters-io/openapi/openwaters-io-currents-api-openapi.yml
- filename: openwaters-io-stations-api-openapi.yml
  format: yaml
  label: Open Waters Stations API
  slug: openwaters-io-stations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openwaters-io/openapi/openwaters-io-stations-api-openapi.yml
- filename: openwaters-io-status-api-openapi.yml
  format: yaml
  label: Open Waters Status API
  slug: openwaters-io-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openwaters-io/openapi/openwaters-io-status-api-openapi.yml
- filename: openwaters-io-tides-api-openapi.yml
  format: yaml
  label: Open Waters Tides API
  slug: openwaters-io-tides-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openwaters-io/openapi/openwaters-io-tides-api-openapi.yml
- filename: openwaters-io-vessels-api-openapi.yml
  format: yaml
  label: Open Waters Vessels API
  slug: openwaters-io-vessels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openwaters-io/openapi/openwaters-io-vessels-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openwaters.io
  spf: true
hosts:
- cert_expires: Dec 26 15:31:36 2026 GMT
  host: openwaters.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Open Waters Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Waters, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Open Waters
provider_slug: openwaters-io
slug: openwaters-io-domain-security
source_filename: openwaters-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openwaters.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 15:31:36 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: openwaters.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/openwaters-io/security/openwaters-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Marine
- Open Source
- Data
- Navigation
---
