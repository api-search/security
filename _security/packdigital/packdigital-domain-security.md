---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: packdigital.com
  spf: true
hosts:
- cert_expires: Oct 15 18:48:25 2026 GMT
  host: packdigital.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 05:39:43 2026 GMT
  host: docs.packdigital.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 02:38:12 2026 GMT
  host: app.packdigital.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Packdigital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Packdigital, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Packdigital
provider_slug: packdigital
slug: packdigital-domain-security
source_filename: packdigital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: packdigital.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 18:48:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.packdigital.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 05:39:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.packdigital.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 02:38:12 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: packdigital.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/packdigital/refs/heads/main/security/packdigital-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Content Management
- Headless Commerce
- Shopify
- Hydrogen
- CMS
- A/B Testing
- GraphQL
- MCP
- Agents
- Storefront
---
