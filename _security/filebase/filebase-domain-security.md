---
api_specs:
- filename: filebase-s3-api-openapi.yml
  format: yaml
  label: Filebase S3-Compatible API
  slug: filebase-s3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filebase/refs/heads/main/openapi/filebase-s3-api-openapi.yml
- filename: filebase-platform-api-openapi.yml
  format: yaml
  label: Filebase Platform API
  slug: filebase-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filebase/refs/heads/main/openapi/filebase-platform-api-openapi.yml
- filename: filebase-ipfs-pinning-service-api-openapi.yml
  format: yaml
  label: Filebase IPFS Pinning Service API
  slug: filebase-ipfs-pinning-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filebase/refs/heads/main/openapi/filebase-ipfs-pinning-service-api-openapi.yml
- filename: filebase-ipfs-rpc-api-openapi.yml
  format: yaml
  label: Filebase IPFS RPC API
  slug: filebase-ipfs-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filebase/refs/heads/main/openapi/filebase-ipfs-rpc-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: filebase.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: filebase.io
  spf: false
hosts:
- cert_expires: Aug 27 20:12:52 2026 GMT
  host: filebase.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 17:26:41 2026 GMT
  host: s3.filebase.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 10 21:13:56 2026 GMT
  host: api.filebase.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Filebase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Filebase, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Filebase
provider_slug: filebase
slug: filebase-domain-security
source_filename: filebase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: filebase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 20:12:52 2026 GMT\n  hsts: false\n- host: s3.filebase.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 17:26:41 2026 GMT\n  hsts: null\n- host: api.filebase.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 21:13:56 2026 GMT\n  hsts: null\ndomains:\n- domain: filebase.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: filebase.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/filebase/refs/heads/main/security/filebase-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Object Storage
- IPFS
- S3-Compatible
- Decentralized Storage
- Pinning
- Web3
- Cloud Storage
- Blockchain
---
