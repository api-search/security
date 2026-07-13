---
api_specs:
- filename: transportapi-openapi.yml
  format: yaml
  label: TransportAPI
  slug: transportapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transportapi/refs/heads/main/openapi/transportapi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: transportapi.com
  spf: true
hosts:
- cert_expires: Sep  9 23:59:59 2026 GMT
  host: www.transportapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 08:04:00 2026 GMT
  host: developer.transportapi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: transportapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Transportapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TransportAPI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: TransportAPI
provider_slug: transportapi
slug: transportapi-domain-security
source_filename: transportapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.transportapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:59:59 2026 GMT\n  hsts: false\n- host: developer.transportapi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 13 08:04:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: transportapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: transportapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transportapi/refs/heads/main/security/transportapi-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Public Transit
- Transport
- UK
- Real-Time
- Journey Planning
- Bus
- Rail
---
