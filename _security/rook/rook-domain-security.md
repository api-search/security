---
api_specs:
- filename: rook-ceph-object-storage-openapi.yml
  format: yaml
  label: Rook Ceph Object Storage API
  slug: rook-ceph-object-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rook/refs/heads/main/openapi/rook-ceph-object-storage-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: rook.io
  spf: true
hosts:
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: rook.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rook Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rook, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Rook
provider_slug: rook
slug: rook-domain-security
source_filename: rook-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rook.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: rook.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rook/refs/heads/main/security/rook-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Block Storage
- CNCF
- Ceph
- Cloud Native
- File Storage
- Graduated
- Kubernetes
- Object Storage
- Orchestration
- Storage
---
