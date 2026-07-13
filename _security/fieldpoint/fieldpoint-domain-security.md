---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fieldpoint.net
  spf: true
hosts:
- cert_expires: Aug 26 13:24:28 2026 GMT
  host: fieldpoint.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.fieldpoint.net
  https: false
kind: domain-security
layout: security
method: probed
name: Fieldpoint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fieldpoint, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fieldpoint
provider_slug: fieldpoint
slug: fieldpoint-domain-security
source_filename: fieldpoint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fieldpoint.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 13:24:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.fieldpoint.net\n  https: false\ndomains:\n- domain: fieldpoint.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fieldpoint/refs/heads/main/security/fieldpoint-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Field Service Management
- Work Orders
- Scheduling
- Dispatching
- Technician Management
- Asset Tracking
- Service Contracts
- Mobile Workforce
- Inventory Management
- Enterprise Software
---
