---
api_specs:
- filename: containerd-metrics-openapi.yml
  format: yaml
  label: Containerd Metrics API
  slug: containerd-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/containerd/refs/heads/main/openapi/containerd-metrics-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: containerd.io
  spf: true
hosts:
- cert_expires: Sep 28 16:34:14 2026 GMT
  host: containerd.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Containerd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Containerd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Containerd
provider_slug: containerd
slug: containerd-domain-security
source_filename: containerd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: containerd.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 16:34:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: containerd.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/containerd/refs/heads/main/security/containerd-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Cloud Native
- Container Runtime
- CRI
- Docker
- gRPC
- Kubernetes
- OCI
---
