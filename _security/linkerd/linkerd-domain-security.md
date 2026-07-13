---
api_specs:
- filename: linkerd-proxy-admin-openapi.yml
  format: yaml
  label: Linkerd Proxy Admin API
  slug: proxy-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkerd/refs/heads/main/openapi/linkerd-proxy-admin-openapi.yml
- filename: linkerd-viz-metrics-openapi.yml
  format: yaml
  label: Linkerd Viz Metrics API
  slug: viz-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkerd/refs/heads/main/openapi/linkerd-viz-metrics-openapi.yml
- filename: linkerd-tap-openapi.yml
  format: yaml
  label: Linkerd Tap API
  slug: tap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkerd/refs/heads/main/openapi/linkerd-tap-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: linkerd.io
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: default.svc
  spf: false
hosts:
- cert_expires: Sep 30 15:31:59 2026 GMT
  host: linkerd.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: kubernetes.default.svc
  https: false
- host: metrics-api.linkerd-viz.svc.cluster.local
  https: false
kind: domain-security
layout: security
method: probed
name: Linkerd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Linkerd, probed live across 3 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Linkerd
provider_slug: linkerd
slug: linkerd-domain-security
source_filename: linkerd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: linkerd.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 15:31:59 2026 GMT\n  hsts: false\n- host: kubernetes.default.svc\n  https: false\n- host: metrics-api.linkerd-viz.svc.cluster.local\n  https: false\ndomains:\n- domain: linkerd.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: default.svc\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linkerd/refs/heads/main/security/linkerd-domain-security.yml
summary_line: TLSv1.3
tags:
- Kubernetes
- mTLS
- Observability
- Security
- Service Mesh
---
