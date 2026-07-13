---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Volvo Cars Connected Vehicle API
  slug: volvo-cars-connected-vehicle-api
  spec_type: OpenAPI
  url: https://developer.volvocars.com/apis/connected-vehicle/v2/specification/
- filename: openapi.yaml
  format: yaml
  label: Volvo Cars Energy API
  slug: volvo-cars-energy-api
  spec_type: OpenAPI
  url: https://developer.volvocars.com/apis/energy/v2/specification/
- filename: openapi.yaml
  format: yaml
  label: Volvo Cars Location API
  slug: volvo-cars-location-api
  spec_type: OpenAPI
  url: https://developer.volvocars.com/apis/location/v1/specification/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: volvocars.com
  spf: true
hosts:
- cert_expires: Sep 29 03:20:44 2026 GMT
  host: developer.volvocars.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 18 23:59:59 2027 GMT
  host: api.volvocars.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Volvo Cars Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Volvo Cars, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Volvo Cars
provider_slug: volvo-cars
slug: volvo-cars-domain-security
source_filename: volvo-cars-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.volvocars.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 03:20:44 2026 GMT\n  hsts: null\n- host: api.volvocars.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 18 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: volvocars.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/volvo-cars/refs/heads/main/security/volvo-cars-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Automotive
- Connected Vehicle
- Electric Vehicles
- Telematics
- Android Automotive
- OEM
- Mobility
---
