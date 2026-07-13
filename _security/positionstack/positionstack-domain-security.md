---
api_specs:
- filename: positionstack-openapi.yml
  format: yaml
  label: positionstack Geocoding API
  slug: positionstack-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/positionstack/refs/heads/main/openapi/positionstack-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: positionstack.com
  spf: true
hosts:
- cert_expires: Oct  9 11:44:19 2026 GMT
  host: positionstack.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 11:44:19 2026 GMT
  host: api.positionstack.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Positionstack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for positionstack, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: positionstack
provider_slug: positionstack
slug: positionstack-domain-security
source_filename: positionstack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: positionstack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 11:44:19 2026 GMT\n  hsts: false\n- host: api.positionstack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 11:44:19 2026 GMT\n  hsts: null\ndomains:\n- domain: positionstack.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/positionstack/refs/heads/main/security/positionstack-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Geocoding
- Reverse Geocoding
- Maps
- Location
- Address Validation
- apilayer
- Public APIs
---
