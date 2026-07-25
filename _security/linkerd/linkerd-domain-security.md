---
api_specs:
- filename: linkerd-discovery-api-openapi.yml
  format: yaml
  label: Linkerd Discovery API
  slug: linkerd-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkerd/refs/heads/main/openapi/linkerd-discovery-api-openapi.yml
- filename: linkerd-edges-api-openapi.yml
  format: yaml
  label: Linkerd Edges API
  slug: linkerd-edges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkerd/refs/heads/main/openapi/linkerd-edges-api-openapi.yml
- filename: linkerd-gateways-api-openapi.yml
  format: yaml
  label: Linkerd Gateways API
  slug: linkerd-gateways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkerd/refs/heads/main/openapi/linkerd-gateways-api-openapi.yml
- filename: linkerd-health-api-openapi.yml
  format: yaml
  label: Linkerd Health API
  slug: linkerd-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkerd/refs/heads/main/openapi/linkerd-health-api-openapi.yml
- filename: linkerd-lifecycle-api-openapi.yml
  format: yaml
  label: Linkerd Lifecycle API
  slug: linkerd-lifecycle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkerd/refs/heads/main/openapi/linkerd-lifecycle-api-openapi.yml
- filename: linkerd-metrics-api-openapi.yml
  format: yaml
  label: Linkerd Metrics API
  slug: linkerd-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkerd/refs/heads/main/openapi/linkerd-metrics-api-openapi.yml
- filename: linkerd-routes-api-openapi.yml
  format: yaml
  label: Linkerd Routes API
  slug: linkerd-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkerd/refs/heads/main/openapi/linkerd-routes-api-openapi.yml
- filename: linkerd-statistics-api-openapi.yml
  format: yaml
  label: Linkerd Statistics API
  slug: linkerd-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkerd/refs/heads/main/openapi/linkerd-statistics-api-openapi.yml
- filename: linkerd-tap-api-openapi.yml
  format: yaml
  label: Linkerd Tap API
  slug: linkerd-tap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkerd/refs/heads/main/openapi/linkerd-tap-api-openapi.yml
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
