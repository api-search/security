---
api_specs:
- filename: uniform-platform-api-openapi.json
  format: json
  label: Uniform Platform API
  slug: uniform-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uniform/refs/heads/main/openapi/uniform-platform-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: uniform.dev
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: uniform.app
  spf: false
hosts:
- cert_expires: Sep 23 07:32:57 2026 GMT
  host: uniform.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 09:20:32 2026 GMT
  host: docs.uniform.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 01:48:02 2026 GMT
  host: uniform.app
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uniform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Uniform, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Uniform
provider_slug: uniform
slug: uniform-domain-security
source_filename: uniform-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uniform.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 07:32:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.uniform.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 09:20:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: uniform.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 01:48:02 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: uniform.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: uniform.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uniform/refs/heads/main/security/uniform-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Digital Experience Platform
- Content Management
- Personalization
- AB Testing
- Composable
- Headless CMS
- AI Agents
- Webhooks
---
