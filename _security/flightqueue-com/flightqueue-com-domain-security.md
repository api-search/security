---
api_specs:
- filename: flightqueue-com-airports-api-openapi.yml
  format: yaml
  label: FlightQueue Airports API
  slug: flightqueue-com-airports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flightqueue-com/openapi/flightqueue-com-airports-api-openapi.yml
- filename: flightqueue-com-alerts-api-openapi.yml
  format: yaml
  label: FlightQueue Alerts API
  slug: flightqueue-com-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flightqueue-com/openapi/flightqueue-com-alerts-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: flightqueue.com
  spf: true
hosts:
- cert_expires: Feb  6 11:04:31 2027 GMT
  host: flightqueue.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FlightQueue Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FlightQueue, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: FlightQueue
provider_slug: flightqueue-com
slug: flightqueue-com-domain-security
source_filename: flightqueue-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flightqueue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 11:04:31 2027 GMT\n  hsts: false\ndomains:\n- domain: flightqueue.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/flightqueue-com/security/flightqueue-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Airport
- Real-Time Data
- Travel
- Aviation
---
