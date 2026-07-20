---
api_specs:
- filename: harmony-service-desk-openapi.json
  format: json
  label: Harmony Service Desk API
  slug: harmony-service-desk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harmony/refs/heads/main/openapi/harmony-service-desk-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: harmony.io
  spf: true
hosts:
- cert_expires: Sep 27 19:16:38 2026 GMT
  host: docs.harmony.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 03:39:41 2026 GMT
  host: api.harmony.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Harmony Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Harmony, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Harmony
provider_slug: harmony
slug: harmony-domain-security
source_filename: harmony-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.harmony.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 19:16:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.harmony.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 03:39:41 2026 GMT\n  hsts: null\ndomains:\n- domain: harmony.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harmony/refs/heads/main/security/harmony-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- IT Service Management
- Service Desk
- Ticketing
- Enterprise Service Management
- AI Agents
- IT Automation
- Help Desk
- Identity
- Company
---
