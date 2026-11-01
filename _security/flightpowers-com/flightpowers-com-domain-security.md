---
api_specs:
- filename: flightpowers-com-account-api-openapi.yml
  format: yaml
  label: flightpowers-com Account API
  slug: flightpowers-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flightpowers-com/openapi/flightpowers-com-account-api-openapi.yml
- filename: flightpowers-com-flights-api-openapi.yml
  format: yaml
  label: flightpowers-com Flights API
  slug: flightpowers-com-flights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flightpowers-com/openapi/flightpowers-com-flights-api-openapi.yml
- filename: flightpowers-com-hotels-api-openapi.yml
  format: yaml
  label: flightpowers-com Hotels API
  slug: flightpowers-com-hotels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flightpowers-com/openapi/flightpowers-com-hotels-api-openapi.yml
- filename: flightpowers-com-verify-api-openapi.yml
  format: yaml
  label: flightpowers-com Verify API
  slug: flightpowers-com-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flightpowers-com/openapi/flightpowers-com-verify-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: flightpowers.com
  spf: true
hosts:
- cert_expires: Dec 16 17:40:21 2026 GMT
  host: flightpowers.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Flightpowers Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for flightpowers-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: flightpowers-com
provider_slug: flightpowers-com
slug: flightpowers-com-domain-security
source_filename: flightpowers-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flightpowers.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 17:40:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: flightpowers.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/flightpowers-com/security/flightpowers-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Travel
- Data
- API
- Flights
- Hotels
---
