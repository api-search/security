---
api_specs:
- filename: supermove-openapi.yml
  format: yaml
  label: Supermove Developer API - New Lead Endpoint
  slug: supermove-developer-api-new-lead-endpoint
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supermove/refs/heads/main/openapi/supermove-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: supermove.com
  spf: true
hosts:
- cert_expires: Sep  5 23:41:24 2026 GMT
  host: help.supermove.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Supermove Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Supermove, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Supermove
provider_slug: supermove
slug: supermove-domain-security
source_filename: supermove-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: help.supermove.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 23:41:24 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\ndomains:\n- domain: supermove.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/supermove/refs/heads/main/security/supermove-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Moving
- Moving Company Software
- Logistics
- Field Service
- Lead Management
- Operations
- Dispatch
- Webhooks
---
