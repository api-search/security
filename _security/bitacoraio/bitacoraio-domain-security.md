---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bitacora.io
  spf: true
hosts:
- cert_expires: Sep 16 22:17:53 2026 GMT
  host: bitacora.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bitacoraio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bitacora.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bitacora.io
provider_slug: bitacoraio
slug: bitacoraio-domain-security
source_filename: bitacoraio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bitacora.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 22:17:53 2026 GMT\n  hsts: false\ndomains:\n- domain: bitacora.io\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitacoraio/refs/heads/main/security/bitacoraio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Field Service
- Field Data Collection
- Construction
- Maintenance
- Operations
- Mobile App
- Offline First
- Analytics
- Reporting
- Task Management
- Latin America
- SaaS
---
