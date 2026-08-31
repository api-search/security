---
api_specs:
- filename: coyote-associated-entities-api-api-openapi.yml
  format: yaml
  label: Coyote Logistics Associated Entities API API
  slug: coyote-associated-entities-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coyote/refs/heads/main/openapi/coyote-associated-entities-api-api-openapi.yml
- filename: coyote-carrier-available-load-apis-api-openapi.yml
  format: yaml
  label: Coyote Logistics Carrier - Available Load APIs API
  slug: coyote-carrier-available-load-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coyote/refs/heads/main/openapi/coyote-carrier-available-load-apis-api-openapi.yml
- filename: coyote-carrier-booking-apis-api-openapi.yml
  format: yaml
  label: Coyote Logistics Carrier - Booking APIs API
  slug: coyote-carrier-booking-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coyote/refs/heads/main/openapi/coyote-carrier-booking-apis-api-openapi.yml
- filename: coyote-carrier-offer-apis-api-openapi.yml
  format: yaml
  label: Coyote Logistics Carrier - Offer APIs API
  slug: coyote-carrier-offer-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coyote/refs/heads/main/openapi/coyote-carrier-offer-apis-api-openapi.yml
- filename: coyote-document-apis-api-openapi.yml
  format: yaml
  label: Coyote Logistics Document APIs API
  slug: coyote-document-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coyote/refs/heads/main/openapi/coyote-document-apis-api-openapi.yml
- filename: coyote-shipper-quoting-apis-api-openapi.yml
  format: yaml
  label: Coyote Logistics Shipper - Quoting APIs API
  slug: coyote-shipper-quoting-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coyote/refs/heads/main/openapi/coyote-shipper-quoting-apis-api-openapi.yml
- filename: coyote-shipper-shipment-apis-api-openapi.yml
  format: yaml
  label: Coyote Logistics Shipper - Shipment APIs API
  slug: coyote-shipper-shipment-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coyote/refs/heads/main/openapi/coyote-shipper-shipment-apis-api-openapi.yml
- filename: coyote-shipper-tracking-apis-api-openapi.yml
  format: yaml
  label: Coyote Logistics Shipper - Tracking APIs API
  slug: coyote-shipper-tracking-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coyote/refs/heads/main/openapi/coyote-shipper-tracking-apis-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: coyote.com
  spf: true
hosts:
- cert_expires: Jul 25 03:17:20 2026 GMT
  host: coyote.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 21 12:46:32 2026 GMT
  host: api2-dev.coyote.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 08:45:16 2026 GMT
  host: api.coyote.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coyote Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coyote Logistics, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Coyote Logistics
provider_slug: coyote
slug: coyote-domain-security
source_filename: coyote-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coyote.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 25 03:17:20 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: api2-dev.coyote.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 12:46:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.coyote.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 08:45:16 2026 GMT\n  hsts: null\ndomains:\n- domain: coyote.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coyote/refs/heads/main/security/coyote-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- freight brokerage
- Logistics
- Truckload
- LTL
- less-than-truckload
- Shipping
- supply chain
- freight quotes
- shipment tracking
- load management
- 3PL
- customs brokerage
- carrier API
- shipper API
---
