---
api_specs:
- filename: comos-gateway-com-actions-api-openapi.yml
  format: yaml
  label: comos-gateway-com Actions API
  slug: comos-gateway-com-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comos-gateway-com/openapi/comos-gateway-com-actions-api-openapi.yml
- filename: comos-gateway-com-tools-api-openapi.yml
  format: yaml
  label: comos-gateway-com Tools API
  slug: comos-gateway-com-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comos-gateway-com/openapi/comos-gateway-com-tools-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: comos-gateway.com
  spf: false
hosts:
- cert_expires: Dec 26 11:56:12 2026 GMT
  host: comos-gateway.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Comos Gateway Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for comos-gateway-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: comos-gateway-com
provider_slug: comos-gateway-com
slug: comos-gateway-com-domain-security
source_filename: comos-gateway-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: comos-gateway.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 11:56:12 2026 GMT\n  hsts: false\ndomains:\n- domain: comos-gateway.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/comos-gateway-com/security/comos-gateway-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Federation
- OnPremise
- Commerce
- API
---
