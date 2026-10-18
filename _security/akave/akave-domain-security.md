---
api_specs:
- filename: akave-buckets-api-openapi.yml
  format: yaml
  label: Akave Buckets API
  slug: akave-buckets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akave/refs/heads/main/openapi/akave-buckets-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: akave.ai
  spf: true
hosts:
- cert_expires: Jan  7 10:25:36 2027 GMT
  host: akave.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Akave Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Akave, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Akave
provider_slug: akave
slug: akave-domain-security
source_filename: akave-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: akave.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 10:25:36 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: akave.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akave/refs/heads/main/security/akave-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Object Storage
- S3 Compatible
- Decentralized Storage
- Cloud Storage
- gRPC
- MCP
---
