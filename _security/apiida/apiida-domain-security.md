---
api_specs:
- filename: apiida-api-control-plane-openapi.yml
  format: yaml
  label: APIIDA API Control Plane
  slug: api-control-plane
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiida/refs/heads/main/openapi/apiida-api-control-plane-openapi.yml
- filename: apiida-api-gateway-manager-openapi.yml
  format: yaml
  label: APIIDA API Gateway Manager
  slug: api-gateway-manager
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiida/refs/heads/main/openapi/apiida-api-gateway-manager-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: apiida.com
  spf: true
hosts:
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: apiida.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: api.apiida.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apiida Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for APIIDA, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: APIIDA
provider_slug: apiida
slug: apiida-domain-security
source_filename: apiida-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apiida.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.apiida.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apiida.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apiida/refs/heads/main/security/apiida-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- API Gateway
- API Management
- Federated API Management
- Governance
- Layer7
---
