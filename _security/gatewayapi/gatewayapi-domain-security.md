---
api_specs:
- filename: gatewayapi-rest-api-openapi.yml
  format: yaml
  label: GatewayAPI REST API
  slug: gatewayapi-rest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gatewayapi/openapi/gatewayapi-rest-api-openapi.yml
- filename: gatewayapi-openapi-generated.yml
  format: yaml
  label: GatewayAPI API
  slug: gatewayapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gatewayapi/openapi/_ae-authored/gatewayapi-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: gatewayapi.com
  spf: true
hosts:
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: gatewayapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gatewayapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GatewayAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: GatewayAPI
provider_slug: gatewayapi
slug: gatewayapi-domain-security
source_filename: gatewayapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gatewayapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gatewayapi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/gatewayapi/security/gatewayapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Messaging
- SMS
- API
- Communications
---
