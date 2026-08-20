---
api_specs:
- filename: cabify-delivery-api-openapi.yml
  format: yaml
  label: Cabify delivery API
  slug: cabify-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cabify/refs/heads/main/openapi/cabify-delivery-api-openapi.yml
- filename: cabify-estimates-api-openapi.yml
  format: yaml
  label: Cabify Estimates API
  slug: cabify-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cabify/refs/heads/main/openapi/cabify-estimates-api-openapi.yml
- filename: cabify-hubs-api-openapi.yml
  format: yaml
  label: Cabify hubs API
  slug: cabify-hubs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cabify/refs/heads/main/openapi/cabify-hubs-api-openapi.yml
- filename: cabify-journeys-api-openapi.yml
  format: yaml
  label: Cabify Journeys API
  slug: cabify-journeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cabify/refs/heads/main/openapi/cabify-journeys-api-openapi.yml
- filename: cabify-label-api-openapi.yml
  format: yaml
  label: Cabify label API
  slug: cabify-label-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cabify/refs/heads/main/openapi/cabify-label-api-openapi.yml
- filename: cabify-labels-api-openapi.yml
  format: yaml
  label: Cabify Labels API
  slug: cabify-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cabify/refs/heads/main/openapi/cabify-labels-api-openapi.yml
- filename: cabify-parcels-api-openapi.yml
  format: yaml
  label: Cabify parcels API
  slug: cabify-parcels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cabify/refs/heads/main/openapi/cabify-parcels-api-openapi.yml
- filename: cabify-sales-api-openapi.yml
  format: yaml
  label: Cabify Sales API
  slug: cabify-sales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cabify/refs/heads/main/openapi/cabify-sales-api-openapi.yml
- filename: cabify-shipment-api-openapi.yml
  format: yaml
  label: Cabify shipment API
  slug: cabify-shipment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cabify/refs/heads/main/openapi/cabify-shipment-api-openapi.yml
- filename: cabify-shipping-types-api-openapi.yml
  format: yaml
  label: Cabify shipping_types API
  slug: cabify-shipping-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cabify/refs/heads/main/openapi/cabify-shipping-types-api-openapi.yml
- filename: cabify-status-api-openapi.yml
  format: yaml
  label: Cabify status API
  slug: cabify-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cabify/refs/heads/main/openapi/cabify-status-api-openapi.yml
- filename: cabify-users-api-openapi.yml
  format: yaml
  label: Cabify users API
  slug: cabify-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cabify/refs/heads/main/openapi/cabify-users-api-openapi.yml
- filename: cabify-webhooks-api-openapi.yml
  format: yaml
  label: Cabify webhooks API
  slug: cabify-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cabify/refs/heads/main/openapi/cabify-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 128 issuewild "letsencrypt.org"
  - 128 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cabify.com
  spf: true
hosts:
- cert_expires: Sep 29 15:28:06 2026 GMT
  host: cabify.com
  hsts: true
  hsts_max_age: 6
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 02:40:20 2026 GMT
  host: developers.cabify.com
  hsts: true
  hsts_max_age: 6
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 15:28:06 2026 GMT
  host: logistics.api.cabify.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cabify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cabify, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Cabify
provider_slug: cabify
slug: cabify-domain-security
source_filename: cabify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cabify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 15:28:06 2026 GMT\n  hsts: true\n  hsts_max_age: 6\n- host: developers.cabify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 02:40:20 2026 GMT\n  hsts: true\n  hsts_max_age: 6\n- host: logistics.api.cabify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 15:28:06 2026 GMT\n  hsts: null\ndomains:\n- domain: cabify.com\n  dnssec: true\n  caa:\n  - 128 issuewild \"letsencrypt.org\"\n  - 128 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cabify/refs/heads/main/security/cabify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Transportation
- Ride Hailing
- Mobility
- Logistics
- Delivery
- Last Mile Delivery
- Webhook
- Authentication
---
