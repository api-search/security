---
api_specs:
- filename: karrio-addresses-api-openapi.yml
  format: yaml
  label: Karrio Addresses API
  slug: karrio-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-addresses-api-openapi.yml
- filename: karrio-api-api-openapi.yml
  format: yaml
  label: Karrio API
  slug: karrio-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-api-api-openapi.yml
- filename: karrio-auth-api-openapi.yml
  format: yaml
  label: Karrio Auth API
  slug: karrio-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-auth-api-openapi.yml
- filename: karrio-batches-api-openapi.yml
  format: yaml
  label: Karrio Batches API
  slug: karrio-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-batches-api-openapi.yml
- filename: karrio-carriers-api-openapi.yml
  format: yaml
  label: Karrio Carriers API
  slug: karrio-carriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-carriers-api-openapi.yml
- filename: karrio-connections-api-openapi.yml
  format: yaml
  label: Karrio Connections API
  slug: karrio-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-connections-api-openapi.yml
- filename: karrio-documents-api-openapi.yml
  format: yaml
  label: Karrio Documents API
  slug: karrio-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-documents-api-openapi.yml
- filename: karrio-manifests-api-openapi.yml
  format: yaml
  label: Karrio Manifests API
  slug: karrio-manifests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-manifests-api-openapi.yml
- filename: karrio-orders-api-openapi.yml
  format: yaml
  label: Karrio Orders API
  slug: karrio-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-orders-api-openapi.yml
- filename: karrio-parcels-api-openapi.yml
  format: yaml
  label: Karrio Parcels API
  slug: karrio-parcels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-parcels-api-openapi.yml
- filename: karrio-pickups-api-openapi.yml
  format: yaml
  label: Karrio Pickups API
  slug: karrio-pickups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-pickups-api-openapi.yml
- filename: karrio-products-api-openapi.yml
  format: yaml
  label: Karrio Products API
  slug: karrio-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-products-api-openapi.yml
- filename: karrio-proxy-api-openapi.yml
  format: yaml
  label: Karrio Proxy API
  slug: karrio-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-proxy-api-openapi.yml
- filename: karrio-shipments-api-openapi.yml
  format: yaml
  label: Karrio Shipments API
  slug: karrio-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-shipments-api-openapi.yml
- filename: karrio-trackers-api-openapi.yml
  format: yaml
  label: Karrio Trackers API
  slug: karrio-trackers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-trackers-api-openapi.yml
- filename: karrio-webhooks-api-openapi.yml
  format: yaml
  label: Karrio Webhooks API
  slug: karrio-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: karrio.io
  spf: false
hosts:
- cert_expires: Oct 30 08:06:14 2026 GMT
  host: karrio.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Karrio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Karrio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Karrio
provider_slug: karrio
slug: karrio-domain-security
source_filename: karrio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: karrio.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 08:06:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: karrio.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/security/karrio-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Shipping
- Logistics
- Label Generation
- Package Tracking
- Carriers
- Fulfillment
- Open Source
- Multi-Carrier
- Rating
- Webhooks
---
