---
api_specs:
- filename: deliverect-pos-api-openapi-original.yml
  format: yaml
  label: Deliverect POS API
  slug: pos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverect/refs/heads/main/openapi/deliverect-pos-api-openapi-original.yml
- filename: deliverect-commerce-api-openapi-original.yml
  format: yaml
  label: Deliverect Commerce API
  slug: commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverect/refs/heads/main/openapi/deliverect-commerce-api-openapi-original.yml
- filename: deliverect-channel-api-openapi-original.yml
  format: yaml
  label: Deliverect Channel API
  slug: channel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverect/refs/heads/main/openapi/deliverect-channel-api-openapi-original.yml
- filename: deliverect-dispatch-api-openapi-original.yml
  format: yaml
  label: Deliverect Dispatch API
  slug: dispatch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverect/refs/heads/main/openapi/deliverect-dispatch-api-openapi-original.yml
- filename: deliverect-store-api-openapi-original.yml
  format: yaml
  label: Deliverect Store API
  slug: store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverect/refs/heads/main/openapi/deliverect-store-api-openapi-original.yml
- filename: deliverect-pay-api-openapi-original.yml
  format: yaml
  label: Deliverect Pay API
  slug: pay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverect/refs/heads/main/openapi/deliverect-pay-api-openapi-original.yml
- filename: deliverect-crm-api-openapi-original.yml
  format: yaml
  label: Deliverect CRM API
  slug: crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverect/refs/heads/main/openapi/deliverect-crm-api-openapi-original.yml
- filename: deliverect-loyalty-api-openapi-original.yml
  format: yaml
  label: Deliverect Loyalty API
  slug: loyalty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverect/refs/heads/main/openapi/deliverect-loyalty-api-openapi-original.yml
- filename: deliverect-kds-api-openapi-original.yml
  format: yaml
  label: Deliverect KDS API
  slug: kds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverect/refs/heads/main/openapi/deliverect-kds-api-openapi-original.yml
- filename: deliverect-gift-cards-api-openapi-original.yml
  format: yaml
  label: Deliverect Gift Cards API
  slug: gift-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverect/refs/heads/main/openapi/deliverect-gift-cards-api-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: deliverect.com
  spf: true
hosts:
- cert_expires: Sep 16 06:45:37 2026 GMT
  host: www.deliverect.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 19:21:00 2026 GMT
  host: developers.deliverect.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 06:45:37 2026 GMT
  host: api.deliverect.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deliverect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deliverect, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Deliverect
provider_slug: deliverect
slug: deliverect-domain-security
source_filename: deliverect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.deliverect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 06:45:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.deliverect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 19:21:00 2026 GMT\n  hsts: null\n- host: api.deliverect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 06:45:37 2026 GMT\n  hsts: null\ndomains:\n- domain: deliverect.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deliverect/refs/heads/main/security/deliverect-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurant
- Delivery
- Online Ordering
- Point of Sale
- Order Management
- Integration
---
