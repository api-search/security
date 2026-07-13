---
api_specs:
- filename: cargosmart-shipment-tracking-openapi.yml
  format: yaml
  label: CargoSmart Container Booking API
  slug: cargosmart-container-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargosmart/refs/heads/main/openapi/cargosmart-shipment-tracking-openapi.yml
- filename: cargosmart-shipment-tracking-openapi.yml
  format: yaml
  label: CargoSmart Shipment Tracking API
  slug: cargosmart-shipment-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargosmart/refs/heads/main/openapi/cargosmart-shipment-tracking-openapi.yml
- filename: cargosmart-shipment-tracking-openapi.yml
  format: yaml
  label: CargoSmart Vessel Schedule API
  slug: cargosmart-vessel-schedule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargosmart/refs/heads/main/openapi/cargosmart-shipment-tracking-openapi.yml
- filename: cargosmart-shipment-tracking-openapi.yml
  format: yaml
  label: CargoSmart Shipping Documentation API
  slug: cargosmart-shipping-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargosmart/refs/heads/main/openapi/cargosmart-shipment-tracking-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cargosmart.com
  spf: true
hosts:
- cert_expires: Dec 13 18:23:36 2026 GMT
  host: www.cargosmart.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 13 18:23:36 2026 GMT
  host: api.cargosmart.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cargosmart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CargoSmart, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: CargoSmart
provider_slug: cargosmart
slug: cargosmart-domain-security
source_filename: cargosmart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cargosmart.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 13 18:23:36 2026 GMT\n  hsts: false\n- host: api.cargosmart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 18:23:36 2026 GMT\n  hsts: null\ndomains:\n- domain: cargosmart.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cargosmart/refs/heads/main/security/cargosmart-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Booking
- Container
- Documentation
- GSBN
- IQAX
- Logistics
- Maritime
- Ocean Freight
- Schedule
- Shipping
- Supply Chain
- Tracking
- Visibility
- Vessel
---
