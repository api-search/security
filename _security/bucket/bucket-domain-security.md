---
api_specs:
- filename: bucket-management-openapi-original.json
  format: json
  label: Reflag Management API
  slug: reflag-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bucket/refs/heads/main/openapi/bucket-management-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: reflag.com
  spf: true
hosts:
- cert_expires: Sep 22 19:07:13 2026 GMT
  host: reflag.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 03:01:27 2026 GMT
  host: docs.reflag.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 15:16:07 2026 GMT
  host: app.reflag.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bucket Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bucket, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bucket
provider_slug: bucket
slug: bucket-domain-security
source_filename: bucket-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reflag.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 19:07:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.reflag.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 03:01:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.reflag.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 15:16:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: reflag.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bucket/refs/heads/main/security/bucket-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Feature Flags
- Feature Management
- Feature Flagging
- Developer Tools
- SaaS
- Entitlements
- Experimentation
- MCP
- Agent Ready
---
