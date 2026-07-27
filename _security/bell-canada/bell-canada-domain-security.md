---
api_specs:
- filename: bell-canada-trouble-ticket-api-openapi.json
  format: json
  label: Bell Canada Trouble Ticket API
  slug: bell-canada-trouble-ticket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bell-canada/refs/heads/main/openapi/bell-canada-trouble-ticket-api-openapi.json
- filename: bell-canada-service-order-api-openapi.json
  format: json
  label: Bell Canada Service Order API
  slug: bell-canada-service-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bell-canada/refs/heads/main/openapi/bell-canada-service-order-api-openapi.json
- filename: bell-canada-resource-inventory-api-openapi.json
  format: json
  label: Bell Canada Resource Inventory Management API
  slug: bell-canada-resource-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bell-canada/refs/heads/main/openapi/bell-canada-resource-inventory-api-openapi.json
- filename: bell-canada-change-management-api-openapi.json
  format: json
  label: Bell Canada Change Management API
  slug: bell-canada-change-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bell-canada/refs/heads/main/openapi/bell-canada-change-management-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bell.ca
  spf: true
hosts:
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: www.bell.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: developer.bell.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Bell Canada Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bell Canada, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bell Canada
provider_slug: bell-canada
slug: bell-canada-domain-security
source_filename: bell-canada-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bell.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.bell.ca\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bell.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bell-canada/refs/heads/main/security/bell-canada-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Telecommunications
- Canada
- Mobile Network Operator
- Broadband
- 5G
- IoT
- TM Forum
- BSS
- OSS
- Network APIs
- CAMARA
- Open Gateway
- Identity Verification
- SIM Swap
- Enterprise
---
