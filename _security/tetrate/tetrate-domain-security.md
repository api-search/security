---
api_specs:
- filename: tetrate-service-bridge-openapi.yml
  format: yaml
  label: Tetrate Service Bridge REST API
  slug: tsb-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tetrate/refs/heads/main/openapi/tetrate-service-bridge-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tetrate.io
  spf: true
hosts:
- cert_expires: Aug 18 19:23:51 2026 GMT
  host: tetrate.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 02:53:53 2026 GMT
  host: docs.tetrate.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tetrate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tetrate, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tetrate
provider_slug: tetrate
slug: tetrate-domain-security
source_filename: tetrate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tetrate.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 19:23:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.tetrate.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 02:53:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tetrate.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tetrate/refs/heads/main/security/tetrate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Enterprise
- Envoy
- Istio
- Kubernetes
- Service Mesh
---
