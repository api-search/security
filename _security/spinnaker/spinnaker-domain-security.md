---
api_specs:
- filename: spinnaker-gate-openapi.yml
  format: yaml
  label: Spinnaker Gate API
  slug: spinnaker-gate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinnaker/refs/heads/main/openapi/spinnaker-gate-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: spinnaker.io
  spf: false
hosts:
- cert_expires: Aug 29 03:13:50 2026 GMT
  host: spinnaker.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spinnaker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spinnaker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Spinnaker
provider_slug: spinnaker
slug: spinnaker-domain-security
source_filename: spinnaker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spinnaker.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 03:13:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: spinnaker.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spinnaker/refs/heads/main/security/spinnaker-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Continuous Delivery
- Containers
- DevOps
- Multi-Cloud
- Pipelines
---
