---
api_specs:
- filename: ci-hub-access-openapi.yml
  format: yaml
  label: CI HUB Access SDK API
  slug: access-sdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ci-hub/refs/heads/main/openapi/ci-hub-access-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ci-hub.com
  spf: true
hosts:
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: live.ci-hub.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: stage.ci-hub.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ci Hub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CI HUB, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: CI HUB
provider_slug: ci-hub
slug: ci-hub-domain-security
source_filename: ci-hub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: live.ci-hub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: stage.ci-hub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ci-hub.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ci-hub/refs/heads/main/security/ci-hub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Digital Asset Management
- Content Management
- Product Information Management
- Integration
- Connectors
- Creative Tools
- Marketing
- Brand Management
- Model Context Protocol
- Cloud Storage
- Germany
---
