---
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: weavegrid.com
  spf: true
hosts:
- cert_expires: Oct  7 20:11:26 2026 GMT
  host: www.weavegrid.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: api.weavegrid.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Weavegrid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WeaveGrid, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: WeaveGrid
provider_slug: weavegrid
slug: weavegrid-domain-security
source_filename: weavegrid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.weavegrid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 20:11:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.weavegrid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: weavegrid.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weavegrid/refs/heads/main/security/weavegrid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Electric Utilities
- Electric Vehicles
- EV Charging
- Smart Grid
- Managed Charging
- Distributed Energy Resources
- Demand Response
- Grid Orchestration
- Vehicle Telematics
- Climate Tech
- Company
---
