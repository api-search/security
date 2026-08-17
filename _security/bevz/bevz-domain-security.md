---
api_specs:
- filename: bevz-integrator-service-openapi.yaml
  format: yaml
  label: Bevz Integrator Service
  slug: bevz-integrator-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bevz/refs/heads/main/openapi/bevz-integrator-service-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bevz.com
  spf: true
hosts:
- cert_expires: Sep 13 04:44:29 2026 GMT
  host: bevz.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: api.bevz.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: sandbox-api.bevz.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bevz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bevz, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bevz
provider_slug: bevz
slug: bevz-domain-security
source_filename: bevz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bevz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 04:44:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: api.bevz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: null\n- host: sandbox-api.bevz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: bevz.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bevz/refs/heads/main/security/bevz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Delivery Management
- Liquor Retail
- Convenience Store
- Point of Sale
- Food Delivery
- Retail Technology
- Marketing
- Menu Management
- Order Management
- Webhooks
- Integrator API
---
