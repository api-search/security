---
api_specs:
- filename: lanzatech-wordpress-openapi.yml
  format: yaml
  label: LanzaTech WordPress REST API
  slug: wordpress
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lanzatech/refs/heads/main/openapi/lanzatech-wordpress-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lanzatech.com
  spf: true
hosts:
- cert_expires: Aug 29 21:49:07 2026 GMT
  host: lanzatech.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lanzatech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LanzaTech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LanzaTech
provider_slug: lanzatech
slug: lanzatech-domain-security
source_filename: lanzatech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lanzatech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 21:49:07 2026 GMT\n  hsts: false\ndomains:\n- domain: lanzatech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lanzatech/refs/heads/main/security/lanzatech-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Carbon Capture
- Climate Tech
- Sustainability
- Synthetic Biology
- Energy
- Chemicals
- Sustainable Aviation Fuel
- Manufacturing
- Content
---
