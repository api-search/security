---
api_specs:
- filename: cri-o-status-openapi.yml
  format: yaml
  label: CRI-O Status API
  slug: cri-o-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cri-o/refs/heads/main/openapi/cri-o-status-openapi.yml
- filename: cri-o-metrics-openapi.yml
  format: yaml
  label: CRI-O Metrics API
  slug: cri-o-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cri-o/refs/heads/main/openapi/cri-o-metrics-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: cri-o.io
  spf: false
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: kubernetes.io
  spf: true
hosts:
- cert_expires: Sep 19 02:13:52 2026 GMT
  host: cri-o.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 09:13:55 2026 GMT
  host: kubernetes.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cri O Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CRI-O, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: CRI-O
provider_slug: cri-o
slug: cri-o-domain-security
source_filename: cri-o-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cri-o.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 02:13:52 2026 GMT\n  hsts: false\n- host: kubernetes.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 09:13:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cri-o.io\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n- domain: kubernetes.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cri-o/refs/heads/main/security/cri-o-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Apache 2.0
- CNCF
- Cloud Native
- conmon
- Container Runtime
- Containers
- CRI
- Go
- Graduated
- Kubernetes
- OCI
- Open Source
- Prometheus
- runc
---
