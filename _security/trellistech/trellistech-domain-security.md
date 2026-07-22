---
api_specs:
- filename: trellistech-public-api.json
  format: json
  label: Trellis Public API
  slug: trellis-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trellistech/refs/heads/main/openapi/trellistech-public-api.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: trellistech.com
  spf: true
hosts:
- cert_expires: Sep 17 02:49:45 2026 GMT
  host: www.trellistech.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 02:49:45 2026 GMT
  host: docs.trellistech.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 01:15:20 2026 GMT
  host: app.trellistech.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trellistech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trellis, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Trellis
provider_slug: trellistech
slug: trellistech-domain-security
source_filename: trellistech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trellistech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 02:49:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.trellistech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 02:49:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.trellistech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 01:15:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: trellistech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trellistech/refs/heads/main/security/trellistech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Property Management
- Vacation Rentals
- Short-Term Rentals
- AI Agents
- Operations
- Hospitality
- Task Management
- Model Context Protocol
---
