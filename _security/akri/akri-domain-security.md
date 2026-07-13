---
api_specs:
- filename: akri-metrics-openapi.yaml
  format: yaml
  label: Akri Metrics API
  slug: metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akri/refs/heads/main/openapi/akri-metrics-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: akri.sh
  spf: false
hosts:
- cert_expires: Sep  3 14:47:44 2026 GMT
  host: docs.akri.sh
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Akri Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Akri, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Akri
provider_slug: akri
slug: akri-domain-security
source_filename: akri-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.akri.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 14:47:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: akri.sh\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akri/refs/heads/main/security/akri-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Device Management
- Edge Computing
- IoT
- Kubernetes
- CNCF
- Open Source
- OPC UA
- ONVIF
- udev
---
