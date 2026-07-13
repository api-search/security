---
api_specs:
- filename: toyota-vehicle-openapi.yml
  format: yaml
  label: Toyota Vehicle API
  slug: toyota-vehicle
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toyota/refs/heads/main/openapi/toyota-vehicle-openapi.yml
- filename: toyota-telematics-openapi.yml
  format: yaml
  label: Toyota Telematics API
  slug: toyota-telematics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toyota/refs/heads/main/openapi/toyota-telematics-openapi.yml
- filename: toyota-connected-services-openapi.yml
  format: yaml
  label: Toyota Connected Services API
  slug: toyota-connected-services
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toyota/refs/heads/main/openapi/toyota-connected-services-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: toyota.com
  spf: true
hosts:
- cert_expires: Oct  5 23:59:59 2026 GMT
  host: developer.eig.toyota.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 23:59:59 2026 GMT
  host: developer-sb.eig.toyota.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: api.toyota.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Toyota Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Toyota, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Toyota
provider_slug: toyota
slug: toyota-domain-security
source_filename: toyota-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.eig.toyota.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:59:59 2026 GMT\n  hsts: null\n- host: developer-sb.eig.toyota.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.toyota.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: toyota.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toyota/refs/heads/main/security/toyota-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automobiles
- Cars
- Vehicles
- Connected Car
- Telematics
- Fleet Management
- Electric Vehicles
---
