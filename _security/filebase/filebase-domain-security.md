---
api_specs:
- filename: filebase-buckets-api-openapi.yml
  format: yaml
  label: Filebase Buckets API
  slug: filebase-buckets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filebase/refs/heads/main/openapi/filebase-buckets-api-openapi.yml
- filename: filebase-data-management-api-openapi.yml
  format: yaml
  label: Filebase Data Management API
  slug: filebase-data-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filebase/refs/heads/main/openapi/filebase-data-management-api-openapi.yml
- filename: filebase-ipns-api-openapi.yml
  format: yaml
  label: Filebase IPNS API
  slug: filebase-ipns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filebase/refs/heads/main/openapi/filebase-ipns-api-openapi.yml
- filename: filebase-keypairs-api-openapi.yml
  format: yaml
  label: Filebase Keypairs API
  slug: filebase-keypairs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filebase/refs/heads/main/openapi/filebase-keypairs-api-openapi.yml
- filename: filebase-mfs-api-openapi.yml
  format: yaml
  label: Filebase MFS API
  slug: filebase-mfs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filebase/refs/heads/main/openapi/filebase-mfs-api-openapi.yml
- filename: filebase-multipart-upload-api-openapi.yml
  format: yaml
  label: Filebase Multipart Upload API
  slug: filebase-multipart-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filebase/refs/heads/main/openapi/filebase-multipart-upload-api-openapi.yml
- filename: filebase-node-api-openapi.yml
  format: yaml
  label: Filebase Node API
  slug: filebase-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filebase/refs/heads/main/openapi/filebase-node-api-openapi.yml
- filename: filebase-objects-api-openapi.yml
  format: yaml
  label: Filebase Objects API
  slug: filebase-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filebase/refs/heads/main/openapi/filebase-objects-api-openapi.yml
- filename: filebase-pinning-api-openapi.yml
  format: yaml
  label: Filebase Pinning API
  slug: filebase-pinning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filebase/refs/heads/main/openapi/filebase-pinning-api-openapi.yml
- filename: filebase-pins-api-openapi.yml
  format: yaml
  label: Filebase Pins API
  slug: filebase-pins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filebase/refs/heads/main/openapi/filebase-pins-api-openapi.yml
- filename: filebase-usage-api-openapi.yml
  format: yaml
  label: Filebase Usage API
  slug: filebase-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filebase/refs/heads/main/openapi/filebase-usage-api-openapi.yml
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
