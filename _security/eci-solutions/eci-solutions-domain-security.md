---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ecisolutions.com
  spf: true
hosts:
- cert_expires: Sep  5 21:31:29 2026 GMT
  host: www.ecisolutions.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eci Solutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ECI Solutions, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ECI Solutions
provider_slug: eci-solutions
slug: eci-solutions-domain-security
source_filename: eci-solutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ecisolutions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 21:31:29 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: ecisolutions.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eci-solutions/refs/heads/main/security/eci-solutions-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accounting
- Business Management
- CRM
- Distribution
- E-Commerce
- ERP
- Field Service
- Inventory
- Manufacturing
- Retail
---
