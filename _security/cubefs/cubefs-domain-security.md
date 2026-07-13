---
api_specs:
- filename: cubefs-s3-api-openapi.yml
  format: yaml
  label: CubeFS S3-Compatible API
  slug: cubefs-s3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cubefs/refs/heads/main/openapi/cubefs-s3-api-openapi.yml
- filename: cubefs-master-api-openapi.yml
  format: yaml
  label: CubeFS Master API
  slug: cubefs-master-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cubefs/refs/heads/main/openapi/cubefs-master-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cubefs.io
  spf: false
hosts:
- cert_expires: Feb 12 23:59:59 2027 GMT
  host: cubefs.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cubefs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CubeFS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: CubeFS
provider_slug: cubefs
slug: cubefs-domain-security
source_filename: cubefs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cubefs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: cubefs.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cubefs/refs/heads/main/security/cubefs-domain-security.yml
summary_line: TLSv1.3
tags:
- Cloud Native
- CNCF Graduated
- Distributed File System
- Kubernetes
- Object Storage
- POSIX
- S3 Compatible
- Storage
---
