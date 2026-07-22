---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: autodesk.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: plangrid.com
  spf: true
hosts:
- cert_expires: Aug 29 20:13:45 2026 GMT
  host: construction.autodesk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 12:10:06 2026 GMT
  host: developer.plangrid.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: io.plangrid.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plangrid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PlanGrid, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: PlanGrid
provider_slug: plangrid
slug: plangrid-domain-security
source_filename: plangrid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: construction.autodesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 20:13:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.plangrid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 12:10:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: io.plangrid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: autodesk.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: plangrid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plangrid/refs/heads/main/security/plangrid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Enterprise
- Construction
- Construction Technology
- Project Management
- Field Reports
- Documents
- RFIs
- REST API
- Autodesk
---
