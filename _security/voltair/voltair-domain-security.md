---
api_specs:
- filename: voltair-api-openapi-original.yml
  format: yaml
  label: Voltair API
  slug: voltair-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/openapi/voltair-api-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: voltairlabs.com
  spf: true
hosts:
- cert_expires: Sep 30 15:21:12 2026 GMT
  host: voltairlabs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: api.voltairlabs.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Voltair Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Voltair, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Voltair
provider_slug: voltair
slug: voltair-domain-security
source_filename: voltair-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: voltairlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 15:21:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.voltairlabs.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: voltairlabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/security/voltair-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Drones
- Earth Observation
- Infrastructure Inspection
- Utilities
- Energy
- Robotics
- LiDAR
- Aerial Imagery
---
