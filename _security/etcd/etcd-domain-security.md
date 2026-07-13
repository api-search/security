---
api_specs:
- filename: etcd-http-gateway-openapi.yml
  format: yaml
  label: etcd HTTP Gateway API
  slug: etcd-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/etcd/refs/heads/main/openapi/etcd-http-gateway-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: etcd.io
  spf: true
hosts:
- cert_expires: Oct  1 03:13:49 2026 GMT
  host: etcd.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Etcd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Etcd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Etcd
provider_slug: etcd
slug: etcd-domain-security
source_filename: etcd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: etcd.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 03:13:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: etcd.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/etcd/refs/heads/main/security/etcd-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Cloud Native
- Consensus
- Distributed Systems
- Graduated
- Key-Value Store
- Kubernetes
---
