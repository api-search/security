---
api_specs:
- filename: rustfs-health-api-openapi.yml
  format: yaml
  label: RustFS Health API
  slug: rustfs-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rustfs/refs/heads/main/openapi/rustfs-health-api-openapi.yml
- filename: rustfs-minio-api-openapi.yml
  format: yaml
  label: RustFS Minio API
  slug: rustfs-minio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rustfs/refs/heads/main/openapi/rustfs-minio-api-openapi.yml
- filename: rustfs-rustfs-api-api-openapi.yml
  format: yaml
  label: RustFS RustFS API
  slug: rustfs-rustfs-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rustfs/refs/heads/main/openapi/rustfs-rustfs-api-api-openapi.yml
- filename: rustfs-rustfs-api-openapi.yml
  format: yaml
  label: RustFS Rustfs API
  slug: rustfs-rustfs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rustfs/refs/heads/main/openapi/rustfs-rustfs-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rustfs.com
  spf: true
hosts:
- cert_expires: Dec 31 13:38:11 2026 GMT
  host: rustfs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rustfs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RustFS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: RustFS
provider_slug: rustfs
slug: rustfs-domain-security
source_filename: rustfs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rustfs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 13:38:11 2026 GMT\n  hsts: false\ndomains:\n- domain: rustfs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rustfs/refs/heads/main/security/rustfs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Object Storage
- S3
- Open Source
- Storage
---
