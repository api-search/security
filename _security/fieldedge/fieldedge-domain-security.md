---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fieldedge.com
  spf: true
hosts:
- cert_expires: Sep  6 11:13:59 2026 GMT
  host: fieldedge.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 18:12:05 2026 GMT
  host: docs.api.fieldedge.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 00:26:37 2026 GMT
  host: api.fieldedge.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fieldedge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FieldEdge, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FieldEdge
provider_slug: fieldedge
slug: fieldedge-domain-security
source_filename: fieldedge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fieldedge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 11:13:59 2026 GMT\n  hsts: false\n- host: docs.api.fieldedge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 18:12:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.fieldedge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 00:26:37 2026 GMT\n  hsts: null\ndomains:\n- domain: fieldedge.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fieldedge/refs/heads/main/security/fieldedge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Field Service Management
- FSM
- HVAC
- Plumbing
- Electrical
- Home Services
- Dispatch
- Work Orders
- Contractors
- Xplor
---
