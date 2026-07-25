---
api_specs:
- filename: shipday-assignment-api-openapi.yml
  format: yaml
  label: Shipday Assignment API
  slug: shipday-assignment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipday/refs/heads/main/openapi/shipday-assignment-api-openapi.yml
- filename: shipday-drivers-api-openapi.yml
  format: yaml
  label: Shipday Drivers API
  slug: shipday-drivers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipday/refs/heads/main/openapi/shipday-drivers-api-openapi.yml
- filename: shipday-on-demand-delivery-api-openapi.yml
  format: yaml
  label: Shipday On-Demand Delivery API
  slug: shipday-on-demand-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipday/refs/heads/main/openapi/shipday-on-demand-delivery-api-openapi.yml
- filename: shipday-orders-api-openapi.yml
  format: yaml
  label: Shipday Orders API
  slug: shipday-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipday/refs/heads/main/openapi/shipday-orders-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: shipday.com
  spf: true
hosts:
- cert_expires: Aug 21 03:35:01 2026 GMT
  host: www.shipday.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 18:13:50 2026 GMT
  host: docs.shipday.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 23:59:59 2026 GMT
  host: api.shipday.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shipday Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shipday, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Shipday
provider_slug: shipday
slug: shipday-domain-security
source_filename: shipday-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shipday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 03:35:01 2026 GMT\n  hsts: false\n- host: docs.shipday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 18:13:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.shipday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: shipday.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shipday/refs/heads/main/security/shipday-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Delivery
- Logistics
- Last Mile
- Local Delivery
- Dispatch
---
