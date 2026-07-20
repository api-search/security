---
api_specs:
- filename: fudo-openapi-original.yml
  format: yaml
  label: Fudo API
  slug: fudo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fudo/refs/heads/main/openapi/fudo-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fu.do
  spf: true
hosts:
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: fu.do
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: dev.fu.do
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: api.fu.do
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fudo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fudo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fudo
provider_slug: fudo
slug: fudo-domain-security
source_filename: fudo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fu.do\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: false\n- host: dev.fu.do\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: false\n- host: api.fu.do\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: fu.do\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fudo/refs/heads/main/security/fudo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Restaurant
- Point of Sale
- Hospitality
- Food and Beverage
- Payments
- Inventory
- Latin America
- SaaS
---
