---
api_specs:
- filename: drone-api-openapi.yml
  format: yaml
  label: Drone REST API
  slug: drone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drone/refs/heads/main/openapi/drone-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: drone.io
  spf: true
hosts:
- cert_expires: Sep 17 20:03:50 2026 GMT
  host: www.drone.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 06:53:48 2026 GMT
  host: docs.drone.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Drone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Drone, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Drone
provider_slug: drone
slug: drone-domain-security
source_filename: drone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.drone.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 20:03:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.drone.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 06:53:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: drone.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drone/refs/heads/main/security/drone-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- CI/CD
- Continuous Integration
- Continuous Delivery
- DevOps
- Containers
- Docker
- Build Automation
- Open Source
- Self-Hosted
---
