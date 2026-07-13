---
api_specs:
- filename: istio-networking-api-openapi.yml
  format: yaml
  label: Istio Networking API
  slug: networking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istio/refs/heads/main/openapi/istio-networking-api-openapi.yml
- filename: istio-security-api-openapi.yml
  format: yaml
  label: Istio Security API
  slug: security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istio/refs/heads/main/openapi/istio-security-api-openapi.yml
- filename: istio-telemetry-api-openapi.yml
  format: yaml
  label: Istio Telemetry API
  slug: telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istio/refs/heads/main/openapi/istio-telemetry-api-openapi.yml
- filename: istio-extensions-api-openapi.yml
  format: yaml
  label: Istio Extensions API
  slug: extensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istio/refs/heads/main/openapi/istio-extensions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: istio.io
  spf: true
hosts:
- cert_expires: Sep 25 03:23:54 2026 GMT
  host: istio.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Istio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Istio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Istio
provider_slug: istio
slug: istio-domain-security
source_filename: istio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: istio.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 03:23:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: istio.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/istio/refs/heads/main/security/istio-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- CNCF
- Kubernetes
- Microservices
- Open Source
- Service Mesh
---
