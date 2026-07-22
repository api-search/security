---
api_specs:
- filename: sonarly-openapi.yml
  format: yaml
  label: Sonarly API
  slug: sonarly-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonarly/refs/heads/main/openapi/sonarly-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sonarly.com
  spf: true
hosts:
- cert_expires: Sep  7 00:11:00 2026 GMT
  host: sonarly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sonarly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sonarly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sonarly
provider_slug: sonarly
slug: sonarly-domain-security
source_filename: sonarly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sonarly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 00:11:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sonarly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sonarly/refs/heads/main/security/sonarly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Reliability
- Observability
- Monitoring
- Bug Detection
- Incident Management
- Root Cause Analysis
- AI Agents
- Developer Tools
- DevOps
---
