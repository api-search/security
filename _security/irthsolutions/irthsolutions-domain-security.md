---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: irthsolutions.com
  spf: true
hosts:
- cert_expires: Sep  4 19:12:23 2026 GMT
  host: irthsolutions.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Irthsolutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Irth Solutions, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Irth Solutions
provider_slug: irthsolutions
slug: irthsolutions-domain-security
source_filename: irthsolutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: irthsolutions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 19:12:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: irthsolutions.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/irthsolutions/refs/heads/main/security/irthsolutions-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Damage Prevention
- 811 Ticket Management
- Utility Locating
- Pipeline Integrity
- Land Management
- Geospatial
- SaaS
- Energy
- Utilities
- Telecom
---
