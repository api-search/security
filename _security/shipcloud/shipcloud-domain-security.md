---
api_specs:
- filename: shipcloud-addresses-api-openapi.yml
  format: yaml
  label: shipcloud Addresses API
  slug: shipcloud-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-addresses-api-openapi.yml
- filename: shipcloud-carriers-api-openapi.yml
  format: yaml
  label: shipcloud Carriers API
  slug: shipcloud-carriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-carriers-api-openapi.yml
- filename: shipcloud-default-returns-address-api-openapi.yml
  format: yaml
  label: shipcloud Default Returns Address API
  slug: shipcloud-default-returns-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-default-returns-address-api-openapi.yml
- filename: shipcloud-default-shipping-address-api-openapi.yml
  format: yaml
  label: shipcloud Default Shipping Address API
  slug: shipcloud-default-shipping-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-default-shipping-address-api-openapi.yml
- filename: shipcloud-invoice-address-api-openapi.yml
  format: yaml
  label: shipcloud Invoice Address API
  slug: shipcloud-invoice-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-invoice-address-api-openapi.yml
- filename: shipcloud-manifests-api-openapi.yml
  format: yaml
  label: shipcloud Manifests API
  slug: shipcloud-manifests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-manifests-api-openapi.yml
- filename: shipcloud-me-api-openapi.yml
  format: yaml
  label: shipcloud Me API
  slug: shipcloud-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-me-api-openapi.yml
- filename: shipcloud-orders-api-openapi.yml
  format: yaml
  label: shipcloud Orders API
  slug: shipcloud-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-orders-api-openapi.yml
- filename: shipcloud-pickup-dropoff-locations-api-openapi.yml
  format: yaml
  label: shipcloud Pickup Dropoff Locations API
  slug: shipcloud-pickup-dropoff-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-pickup-dropoff-locations-api-openapi.yml
- filename: shipcloud-pickup-requests-api-openapi.yml
  format: yaml
  label: shipcloud Pickup Requests API
  slug: shipcloud-pickup-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-pickup-requests-api-openapi.yml
- filename: shipcloud-shipment-quotes-api-openapi.yml
  format: yaml
  label: shipcloud Shipment Quotes API
  slug: shipcloud-shipment-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-shipment-quotes-api-openapi.yml
- filename: shipcloud-shipments-api-openapi.yml
  format: yaml
  label: shipcloud Shipments API
  slug: shipcloud-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-shipments-api-openapi.yml
- filename: shipcloud-trackers-api-openapi.yml
  format: yaml
  label: shipcloud Trackers API
  slug: shipcloud-trackers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-trackers-api-openapi.yml
- filename: shipcloud-webhooks-api-openapi.yml
  format: yaml
  label: shipcloud Webhooks API
  slug: shipcloud-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/openapi/shipcloud-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: shipcloud.io
  spf: true
hosts:
- host: www.shipcloud.io
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Shipcloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for shipcloud, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: shipcloud
provider_slug: shipcloud
slug: shipcloud-domain-security
source_filename: shipcloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shipcloud.io\n  https: false\ndomains:\n- domain: shipcloud.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shipcloud/refs/heads/main/security/shipcloud-domain-security.yml
summary_line: DMARC
tags:
- Company
- Shipping
- Logistics
- Carriers
- Labels
- Tracking
- E-Commerce
---
