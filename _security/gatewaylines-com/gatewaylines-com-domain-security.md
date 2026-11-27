---
api_specs:
- filename: gatewaylines-com-openapi-generated.yml
  format: yaml
  label: Gateway Lines API
  slug: gatewaylines-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gatewaylines-com/openapi/_ae-authored/gatewaylines-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: gatewaylines.com
  spf: true
hosts:
- cert_expires: Jan 12 04:43:18 2027 GMT
  host: gatewaylines.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gateway Lines Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gateway Lines, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Gateway Lines
provider_slug: gatewaylines-com
slug: gatewaylines-com-domain-security
source_filename: gatewaylines-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gatewaylines.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 04:43:18 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gatewaylines.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/gatewaylines-com/security/gatewaylines-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Ocean Freight
- Logistics
- NVOCC
- Shipping
---
