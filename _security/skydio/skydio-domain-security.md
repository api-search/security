---
api_specs:
- filename: skydio-openapi.yml
  format: yaml
  label: Skydio Cloud API
  slug: skydio-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skydio/refs/heads/main/openapi/skydio-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: skydio.com
  spf: true
hosts:
- cert_expires: Sep 24 03:58:51 2026 GMT
  host: www.skydio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 14:33:14 2026 GMT
  host: apidocs.skydio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 11:50:00 2026 GMT
  host: api.skydio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Skydio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Skydio, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Skydio
provider_slug: skydio
slug: skydio-domain-security
source_filename: skydio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.skydio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 03:58:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidocs.skydio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 14:33:14 2026 GMT\n  hsts: null\n- host: api.skydio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 11:50:00 2026 GMT\n  hsts: null\ndomains:\n- domain: skydio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skydio/refs/heads/main/security/skydio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Autonomous Systems
- Defense
- Drones
- Enterprise
- Fleet Management
- Public Safety
- Robotics
- Unmanned Aerial Vehicles
---
