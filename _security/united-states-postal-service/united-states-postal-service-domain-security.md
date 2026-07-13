---
api_specs:
- filename: united-states-postal-service-addresses-openapi.yml
  format: yaml
  label: USPS Addresses API
  slug: usps-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-postal-service/refs/heads/main/openapi/united-states-postal-service-addresses-openapi.yml
- filename: united-states-postal-service-tracking-openapi.yml
  format: yaml
  label: USPS Tracking API
  slug: usps-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-postal-service/refs/heads/main/openapi/united-states-postal-service-tracking-openapi.yml
- filename: united-states-postal-service-domestic-prices-openapi.yml
  format: yaml
  label: USPS Domestic Prices API
  slug: usps-domestic-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-postal-service/refs/heads/main/openapi/united-states-postal-service-domestic-prices-openapi.yml
- filename: united-states-postal-service-carrier-pickup-openapi.yml
  format: yaml
  label: USPS Carrier Pickup API
  slug: usps-carrier-pickup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-postal-service/refs/heads/main/openapi/united-states-postal-service-carrier-pickup-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: usps.com
  spf: true
hosts:
- cert_expires: Nov 16 23:59:59 2026 GMT
  host: developers.usps.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 16 23:59:59 2026 GMT
  host: apis.usps.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 23 23:59:59 2026 GMT
  host: apis-tem.usps.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: United States Postal Service Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for United States Postal Service, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: United States Postal Service
provider_slug: united-states-postal-service
slug: united-states-postal-service-domain-security
source_filename: united-states-postal-service-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.usps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apis.usps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 23:59:59 2026 GMT\n  hsts: null\n- host: apis-tem.usps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: usps.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/united-states-postal-service/refs/heads/main/security/united-states-postal-service-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Government
- Postal Service
- Shipping
- Logistics
- Address Validation
- Package Tracking
---
