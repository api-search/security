---
api_specs:
- filename: warpstream-management-openapi.yml
  format: yaml
  label: WarpStream Management API
  slug: warpstream-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/warpstream/refs/heads/main/openapi/warpstream-management-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: warpstream.com
  spf: true
hosts:
- cert_expires: Sep 11 18:21:19 2026 GMT
  host: www.warpstream.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 12:43:19 2026 GMT
  host: docs.warpstream.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: api.warpstream.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Warpstream Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WarpStream, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: WarpStream
provider_slug: warpstream
slug: warpstream-domain-security
source_filename: warpstream-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.warpstream.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 18:21:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.warpstream.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 12:43:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.warpstream.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: warpstream.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/warpstream/refs/heads/main/security/warpstream-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Kafka
- Streaming
- Serverless
- Object Storage
- BYOC
- Data Streaming
- Apache Kafka
- Message Queue
- Event Streaming
---
