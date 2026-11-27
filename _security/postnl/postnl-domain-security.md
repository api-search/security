---
api_specs:
- filename: postnl-shipment-api-openapi.yml
  format: yaml
  label: PostNL Shipment API v4
  slug: shipment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postnl/openapi/postnl-shipment-api-openapi.yml
- filename: postnl-barcode-api-openapi.yml
  format: yaml
  label: PostNL Barcode API
  slug: barcode-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postnl/openapi/postnl-barcode-api-openapi.yml
- filename: postnl-confirming-api-openapi.yml
  format: yaml
  label: PostNL Confirming API
  slug: confirming-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postnl/openapi/postnl-confirming-api-openapi.yml
- filename: postnl-labelling-api-openapi.yml
  format: yaml
  label: PostNL Labelling API
  slug: labelling-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postnl/openapi/postnl-labelling-api-openapi.yml
- filename: postnl-shippingstatus-api-openapi.yml
  format: yaml
  label: PostNL Shipping Status API
  slug: shippingstatus-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postnl/openapi/postnl-shippingstatus-api-openapi.yml
- filename: postnl-checkout-api-openapi.yml
  format: yaml
  label: PostNL Checkout API
  slug: checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postnl/openapi/postnl-checkout-api-openapi.yml
- filename: postnl-postalcode-check-api-openapi.yml
  format: yaml
  label: PostNL Checkout Postalcode Check API
  slug: postalcode-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postnl/openapi/postnl-postalcode-check-api-openapi.yml
- filename: postnl-deliverydate-api-openapi.yml
  format: yaml
  label: PostNL Deliverydate API
  slug: deliverydate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postnl/openapi/postnl-deliverydate-api-openapi.yml
- filename: postnl-locations-api-openapi.yml
  format: yaml
  label: PostNL Locations API
  slug: locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postnl/openapi/postnl-locations-api-openapi.yml
- filename: postnl-timeframes-api-openapi.yml
  format: yaml
  label: PostNL Timeframes API
  slug: timeframes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postnl/openapi/postnl-timeframes-api-openapi.yml
- filename: postnl-consigments-api-openapi.yml
  format: yaml
  label: PostNL Consigments API
  slug: postnl-consigments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postnl/openapi/postnl-consigments-api-openapi.yml
- filename: postnl-address-api-openapi.yml
  format: yaml
  label: PostNL Address API
  slug: postnl-address-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postnl/openapi/postnl-address-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: postnl.nl
  spf: true
hosts:
- cert_expires: Jan 20 07:44:50 2027 GMT
  host: api-sandbox.postnl.nl
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  3 10:49:54 2027 GMT
  host: api.postnl.nl
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: PostNL Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PostNL, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: PostNL
provider_slug: postnl
slug: postnl-domain-security
source_filename: postnl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api-sandbox.postnl.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 07:44:50 2027 GMT\n  hsts: null\n- host: api.postnl.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 10:49:54 2027 GMT\n  hsts: null\ndomains:\n- domain: postnl.nl\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/postnl/security/postnl-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Shipping
- Logistics
- Postal
- Netherlands
- Parcel
- Address Validation
- E-Commerce
---
