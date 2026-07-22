---
api_specs:
- filename: ninox-public-openapi-original.json
  format: json
  label: Ninox Public API
  slug: ninox-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ninox/refs/heads/main/openapi/ninox-public-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ninox.com
  spf: true
hosts:
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: ninox.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 18:43:11 2026 GMT
  host: docs.ninox.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 11:36:26 2026 GMT
  host: go.ninox.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ninox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ninox, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ninox
provider_slug: ninox
slug: ninox-domain-security
source_filename: ninox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ninox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.ninox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 18:43:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: go.ninox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 11:36:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ninox.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ninox/refs/heads/main/security/ninox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Low-Code
- Database
- No-Code
- Application Development
- Workflow Automation
- Business Apps
- Productivity
---
