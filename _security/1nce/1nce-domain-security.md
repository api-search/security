---
api_specs:
- filename: 1nce-authorization-openapi.yml
  format: yaml
  label: 1NCE Authorization API
  slug: 1nce-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1nce/refs/heads/main/openapi/1nce-authorization-openapi.yml
- filename: 1nce-sim-management-openapi.yml
  format: yaml
  label: 1NCE SIM Management API
  slug: 1nce-sim-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1nce/refs/heads/main/openapi/1nce-sim-management-openapi.yml
- filename: 1nce-os-openapi.yml
  format: yaml
  label: 1NCE OS API
  slug: 1nce-os-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1nce/refs/heads/main/openapi/1nce-os-openapi.yml
- filename: 1nce-order-management-openapi.yml
  format: yaml
  label: 1NCE Order Management API
  slug: 1nce-order-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1nce/refs/heads/main/openapi/1nce-order-management-openapi.yml
- filename: 1nce-product-information-openapi.yml
  format: yaml
  label: 1NCE Product Information API
  slug: 1nce-product-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1nce/refs/heads/main/openapi/1nce-product-information-openapi.yml
- filename: 1nce-support-management-openapi.yml
  format: yaml
  label: 1NCE Support Management API
  slug: 1nce-support-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1nce/refs/heads/main/openapi/1nce-support-management-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 1nce.com
  spf: true
hosts:
- cert_expires: Oct  8 19:40:53 2026 GMT
  host: www.1nce.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 10:52:21 2026 GMT
  host: portal.1nce.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: help.1nce.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 1Nce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 1NCE, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 1NCE
provider_slug: 1nce
slug: 1nce-domain-security
source_filename: 1nce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.1nce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 19:40:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: portal.1nce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 10:52:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.1nce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: 1nce.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1nce/refs/heads/main/security/1nce-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- IoT
- Connectivity
- SIM
- Cellular
- NB-IoT
- LTE-M
- eUICC
- Edge
- Embedded
- Global Roaming
---
