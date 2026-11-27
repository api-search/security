---
api_specs:
- filename: aviasurf-com-health-api-openapi.yml
  format: yaml
  label: Aviasurf Health API
  slug: aviasurf-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aviasurf-com/openapi/aviasurf-com-health-api-openapi.yml
- filename: aviasurf-com-prices-api-openapi.yml
  format: yaml
  label: Aviasurf Prices API
  slug: aviasurf-com-prices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aviasurf-com/openapi/aviasurf-com-prices-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aviasurf.com
  spf: true
hosts:
- cert_expires: Dec 10 23:38:32 2026 GMT
  host: aviasurf.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aviasurf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aviasurf, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aviasurf
provider_slug: aviasurf-com
slug: aviasurf-com-domain-security
source_filename: aviasurf-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aviasurf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:38:32 2026 GMT\n  hsts: false\ndomains:\n- domain: aviasurf.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/aviasurf-com/security/aviasurf-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Flights
- Travel
- Metasearch
- Booking
- Airlines
---
