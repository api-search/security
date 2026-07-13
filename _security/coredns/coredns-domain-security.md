---
api_specs:
- filename: coredns-health-openapi.yml
  format: yaml
  label: CoreDNS Health API
  slug: coredns-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coredns/refs/heads/main/openapi/coredns-health-openapi.yml
- filename: coredns-metrics-openapi.yml
  format: yaml
  label: CoreDNS Metrics API
  slug: coredns-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coredns/refs/heads/main/openapi/coredns-metrics-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: coredns.io
  spf: false
hosts:
- cert_expires: Sep 30 23:54:02 2026 GMT
  host: coredns.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coredns Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoreDNS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: CoreDNS
provider_slug: coredns
slug: coredns-domain-security
source_filename: coredns-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coredns.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:54:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: coredns.io\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coredns/refs/heads/main/security/coredns-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Apache 2.0
- Cloud Native
- CNCF
- DNS
- Go
- Graduated
- Kubernetes
- Networking
- Open Source
- Plugins
- Prometheus
- Service Discovery
---
