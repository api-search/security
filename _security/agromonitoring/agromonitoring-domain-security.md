---
api_specs:
- filename: agromonitoring-openapi.yml
  format: yaml
  label: Agromonitoring
  slug: agromonitoring
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agromonitoring/refs/heads/main/openapi/agromonitoring-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agromonitoring.com
  spf: false
hosts:
- cert_expires: Sep  1 07:15:24 2026 GMT
  host: agromonitoring.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  8 23:59:59 2026 GMT
  host: api.agromonitoring.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Agromonitoring Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agromonitoring, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Agromonitoring
provider_slug: agromonitoring
slug: agromonitoring-domain-security
source_filename: agromonitoring-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agromonitoring.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 07:15:24 2026 GMT\n  hsts: false\n- host: api.agromonitoring.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug  8 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: agromonitoring.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agromonitoring/refs/heads/main/security/agromonitoring-domain-security.yml
summary_line: TLSv1.3
tags:
- Agriculture
- Satellite Imagery
- Vegetation Indices
- Weather
- Precision Agriculture
- Remote Sensing
---
