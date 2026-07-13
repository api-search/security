---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: autodesk.com
  spf: true
hosts:
- cert_expires: Aug 29 20:13:45 2026 GMT
  host: construction.autodesk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: aps.autodesk.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 23:59:59 2026 GMT
  host: developer.api.autodesk.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Autodesk Bim360 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Autodesk BIM 360, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Autodesk BIM 360
provider_slug: autodesk-bim360
slug: autodesk-bim360-domain-security
source_filename: autodesk-bim360-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: construction.autodesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 20:13:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: aps.autodesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: developer.api.autodesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: autodesk.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autodesk-bim360/refs/heads/main/security/autodesk-bim360-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Construction
- Project Management
- BIM
- Document Management
- Field Management
- Issues Tracking
- Cost Management
- Model Coordination
- RFIs
- Checklists
---
