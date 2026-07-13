---
api_specs:
- filename: sendle-orders-api-openapi.yml
  format: yaml
  label: Sendle Orders API
  slug: sendle-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendle/refs/heads/main/openapi/sendle-orders-api-openapi.yml
- filename: sendle-products-api-openapi.yml
  format: yaml
  label: Sendle Products & Quoting API
  slug: sendle-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendle/refs/heads/main/openapi/sendle-products-api-openapi.yml
- filename: sendle-tracking-api-openapi.yml
  format: yaml
  label: Sendle Tracking API
  slug: sendle-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendle/refs/heads/main/openapi/sendle-tracking-api-openapi.yml
- filename: sendle-manifests-api-openapi.yml
  format: yaml
  label: Sendle Shipping Manifests API
  slug: sendle-manifests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendle/refs/heads/main/openapi/sendle-manifests-api-openapi.yml
- filename: sendle-ping-api-openapi.yml
  format: yaml
  label: Sendle Ping API
  slug: sendle-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendle/refs/heads/main/openapi/sendle-ping-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sendle.com
  spf: true
hosts:
- cert_expires: Sep 12 03:10:19 2026 GMT
  host: www.sendle.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 10:44:23 2026 GMT
  host: developers.sendle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.sendle.com
  https: false
kind: domain-security
layout: security
method: probed
name: Sendle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sendle, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sendle
provider_slug: sendle
slug: sendle-domain-security
source_filename: sendle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sendle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 03:10:19 2026 GMT\n  hsts: null\n- host: developers.sendle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 10:44:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sendle.com\n  https: false\ndomains:\n- domain: sendle.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sendle/refs/heads/main/security/sendle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Shipping
- Logistics
- Last Mile
- Parcels
- E-commerce
- Carbon Neutral
- Small Business
- Australia
- United States
- Canada
---
