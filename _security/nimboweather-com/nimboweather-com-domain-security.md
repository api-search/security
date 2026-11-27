---
api_specs:
- filename: nimboweather-com-frames-api-openapi.yml
  format: yaml
  label: Nimbo Weather Frames API
  slug: nimboweather-com-frames-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nimboweather-com/openapi/nimboweather-com-frames-api-openapi.yml
- filename: nimboweather-com-keys-api-openapi.yml
  format: yaml
  label: Nimbo Weather Keys API
  slug: nimboweather-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nimboweather-com/openapi/nimboweather-com-keys-api-openapi.yml
- filename: nimboweather-com-nowcast-api-openapi.yml
  format: yaml
  label: Nimbo Weather Nowcast API
  slug: nimboweather-com-nowcast-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nimboweather-com/openapi/nimboweather-com-nowcast-api-openapi.yml
- filename: nimboweather-com-status-api-openapi.yml
  format: yaml
  label: Nimbo Weather Status API
  slug: nimboweather-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nimboweather-com/openapi/nimboweather-com-status-api-openapi.yml
- filename: nimboweather-com-tiles-api-openapi.yml
  format: yaml
  label: Nimbo Weather Tiles API
  slug: nimboweather-com-tiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nimboweather-com/openapi/nimboweather-com-tiles-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nimboweather.com
  spf: true
hosts:
- cert_expires: Feb 11 13:19:33 2027 GMT
  host: nimboweather.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nimbo Weather Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nimbo Weather, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nimbo Weather
provider_slug: nimboweather-com
slug: nimboweather-com-domain-security
source_filename: nimboweather-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nimboweather.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 13:19:33 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nimboweather.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/nimboweather-com/security/nimboweather-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Weather
- Rain
- Europe
- Forecast
---
