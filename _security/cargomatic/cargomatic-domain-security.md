---
api_specs:
- filename: cargomatic-openapi-original.yml
  format: yaml
  label: Cargomatic Public API
  slug: cargomatic-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargomatic/refs/heads/main/openapi/cargomatic-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cargomatic.com
  spf: true
hosts:
- cert_expires: Aug 16 05:24:06 2026 GMT
  host: cargomatic.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 17:43:17 2026 GMT
  host: api-docs.cargomatic.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 17:43:17 2026 GMT
  host: api.cargomatic.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cargomatic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cargomatic, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cargomatic
provider_slug: cargomatic
slug: cargomatic-domain-security
source_filename: cargomatic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cargomatic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 05:24:06 2026 GMT\n  hsts: null\n- host: api-docs.cargomatic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 17:43:17 2026 GMT\n  hsts: false\n- host: api.cargomatic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 17:43:17 2026 GMT\n  hsts: null\ndomains:\n- domain: cargomatic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cargomatic/refs/heads/main/security/cargomatic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Logistics
- Freight
- Drayage
- Transportation
- Supply Chain
- Shipping
- Trucking
- Marketplace
- Intermodal
---
