---
api_specs:
- filename: contour-httpproxy-openapi.yml
  format: yaml
  label: Contour HTTPProxy API
  slug: contour-httpproxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contour/refs/heads/main/openapi/contour-httpproxy-openapi.yml
- filename: contour-gateway-openapi.yml
  format: yaml
  label: Contour Gateway API
  slug: contour-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contour/refs/heads/main/openapi/contour-gateway-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: projectcontour.io
  spf: false
hosts:
- cert_expires: Sep 24 02:36:35 2026 GMT
  host: projectcontour.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Contour Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Contour, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Contour
provider_slug: contour
slug: contour-domain-security
source_filename: contour-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: projectcontour.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 02:36:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: projectcontour.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contour/refs/heads/main/security/contour-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Envoy
- Ingress Controller
- Kubernetes
- Networking
- Proxy
---
