---
api_specs:
- filename: travelport-openapi.yml
  format: yaml
  label: Travelport TripServices Flights API
  slug: trip-services-flights
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/openapi/travelport-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: travelport.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: travelport.net
  spf: false
hosts:
- cert_expires: Aug 29 06:23:43 2026 GMT
  host: www.travelport.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 11:02:52 2026 GMT
  host: developer.travelport.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 22 23:59:59 2026 GMT
  host: api.travelport.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Travelport Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Travelport, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Travelport
provider_slug: travelport
slug: travelport-domain-security
source_filename: travelport-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.travelport.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 06:23:43 2026 GMT\n  hsts: false\n- host: developer.travelport.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 11:02:52 2026 GMT\n  hsts: false\n- host: api.travelport.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: travelport.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: travelport.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/travelport/refs/heads/main/security/travelport-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Travel
- Travel Technology
- Reservations
- GDS
- NDC
- Flights
- Hotels
- Payments
---
