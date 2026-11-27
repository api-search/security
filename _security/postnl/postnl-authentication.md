---
anonymous_access: false
api_key_in:
- header
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
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: PostNL Authentication
name_suffix: Authentication
oauth_flows: []
overview: PostNL secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PostNL
provider_slug: postnl
scheme_count: 1
schemes:
- in: header
  name: apikey
  parameter: apikey
  sources:
  - openapi/postnl-address-benelux-api-openapi.yml
  - openapi/postnl-address-insight-api-openapi.yml
  - openapi/postnl-address-international-api-openapi.yml
  - openapi/postnl-address-netherlands-api-openapi.yml
  - openapi/postnl-barcode-api-openapi.yml
  - openapi/postnl-checkout-api-openapi.yml
  - openapi/postnl-company-check-api-openapi.yml
  - openapi/postnl-confirming-api-openapi.yml
  - openapi/postnl-deliverydate-api-openapi.yml
  - openapi/postnl-labelling-api-openapi.yml
  - openapi/postnl-locations-api-openapi.yml
  - openapi/postnl-postalcode-check-api-openapi.yml
  - openapi/postnl-shipment-api-openapi.yml
  - openapi/postnl-shippingstatus-api-openapi.yml
  - openapi/postnl-timeframes-api-openapi.yml
  type: apiKey
slug: postnl-authentication
source_filename: postnl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: searched\nsource:\n- https://developer.postnl.nl/support/api-key/how-do-i-get-an-api-key/\n- https://developer.postnl.nl/support/api-key/why-is-my-api-key-not-working/\n- https://developer.postnl.nl/integration-with-postnl/request-api-key/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apikey\n  type: apiKey\n  in: header\n  parameter: apikey\n  sources:\n  - openapi/postnl-address-benelux-api-openapi.yml\n  - openapi/postnl-address-insight-api-openapi.yml\n  - openapi/postnl-address-international-api-openapi.yml\n  - openapi/postnl-address-netherlands-api-openapi.yml\n  - openapi/postnl-barcode-api-openapi.yml\n  - openapi/postnl-checkout-api-openapi.yml\n  - openapi/postnl-company-check-api-openapi.yml\n  - openapi/postnl-confirming-api-openapi.yml\n  - openapi/postnl-deliverydate-api-openapi.yml\n  - openapi/postnl-labelling-api-openapi.yml\n  - openapi/postnl-locations-api-openapi.yml\n  - openapi/postnl-postalcode-check-api-openapi.yml\n\
  \  - openapi/postnl-shipment-api-openapi.yml\n  - openapi/postnl-shippingstatus-api-openapi.yml\n  - openapi/postnl-timeframes-api-openapi.yml\nderived_from: openapi/postnl-address-benelux-api-openapi.yml, openapi/postnl-address-insight-api-openapi.yml, openapi/postnl-address-international-api-openapi.yml, openapi/postnl-address-netherlands-api-openapi.yml,\n  openapi/postnl-barcode-api-openapi.yml, openapi/postnl-checkout-api-openapi.yml, openapi/postnl-company-check-api-openapi.yml, openapi/postnl-confirming-api-openapi.yml, openapi/postnl-deliverydate-api-openapi.yml,\n  openapi/postnl-labelling-api-openapi.yml, openapi/postnl-locations-api-openapi.yml, openapi/postnl-postalcode-check-api-openapi.yml ...\ndocs: https://developer.postnl.nl/support/api-key/how-do-i-get-an-api-key/\nonboarding:\n  issuance: PostNL customers create an integration in Mijn PostNL Zakelijk (My Account > API Management); each integration is issued a sandbox key and a production key.\n  production_gate: For\
  \ future-proof APIs that confirm and label (return) shipments, only the sandbox key is released first; production access is enabled after PostNL technical support validates the sandbox\n    requests.\n  non_customers: Please be aware that developer keys can no longer be issued\n  binding: 'Keys are linked to customer credentials (Customer Code, Customer Number, Barcode Type) and to the environment: a production key only calls the production endpoint.'\n"
source_yaml_url: https://artifacts.apis.io/postnl/authentication/postnl-authentication.yml
summary_line: apiKey · 1 scheme
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
