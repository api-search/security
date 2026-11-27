---
anonymous_access: false
api_key_in: []
api_specs:
- filename: pagaconquickpay-com-cobros-api-openapi.yml
  format: yaml
  label: QuickPay Cobros API
  slug: pagaconquickpay-com-cobros-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagaconquickpay-com/openapi/pagaconquickpay-com-cobros-api-openapi.yml
- filename: pagaconquickpay-com-configuraci-n-api-openapi.yml
  format: yaml
  label: QuickPay Configuración API
  slug: pagaconquickpay-com-configuraci-n-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagaconquickpay-com/openapi/pagaconquickpay-com-configuraci-n-api-openapi.yml
- filename: pagaconquickpay-com-consultas-api-openapi.yml
  format: yaml
  label: QuickPay Consultas API
  slug: pagaconquickpay-com-consultas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagaconquickpay-com/openapi/pagaconquickpay-com-consultas-api-openapi.yml
- filename: pagaconquickpay-com-links-de-cobro-api-openapi.yml
  format: yaml
  label: QuickPay Links de cobro API
  slug: pagaconquickpay-com-links-de-cobro-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagaconquickpay-com/openapi/pagaconquickpay-com-links-de-cobro-api-openapi.yml
- filename: pagaconquickpay-com-onboarding-api-openapi.yml
  format: yaml
  label: QuickPay Onboarding API
  slug: pagaconquickpay-com-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagaconquickpay-com/openapi/pagaconquickpay-com-onboarding-api-openapi.yml
- filename: pagaconquickpay-com-pagos-api-openapi.yml
  format: yaml
  label: QuickPay Pagos API
  slug: pagaconquickpay-com-pagos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagaconquickpay-com/openapi/pagaconquickpay-com-pagos-api-openapi.yml
- filename: pagaconquickpay-com-webhooks-api-openapi.yml
  format: yaml
  label: QuickPay Webhooks API
  slug: pagaconquickpay-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagaconquickpay-com/openapi/pagaconquickpay-com-webhooks-api-openapi.yml
- filename: pagaconquickpay-com-whatsapp-flows-kit-t2-api-openapi.yml
  format: yaml
  label: QuickPay WhatsApp Flows (Kit T2) API
  slug: pagaconquickpay-com-whatsapp-flows-kit-t2-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagaconquickpay-com/openapi/pagaconquickpay-com-whatsapp-flows-kit-t2-api-openapi.yml
auth_types: []
description: Authentication methods as published on the QuickPay documentation pages.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: QuickPay Authentication
name_suffix: Authentication
oauth_flows: []
overview: QuickPay declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: QuickPay
provider_slug: pagaconquickpay-com
scheme_count: 1
schemes:
- evidence: '-H "x-switch-key: $QP_KEY"'
  header: x-switch-key
  how_to_obtain: Create API key in portal under Integraciones › Llaves de API › Crear llave, choose Prueba and copy the value.
  location: header
  name: x-switch-key
  type: apiKey
slug: pagaconquickpay-com-authentication
source_filename: pagaconquickpay-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.pagaconquickpay.com/developers/quickstart.md
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.pagaconquickpay.com/developers/quickstart.md\nsources:\n- https://docs.pagaconquickpay.com/developers/quickstart.md\n- https://docs.pagaconquickpay.com/developers/quickstart\ndescription: Authentication methods as published on the QuickPay documentation pages.\nschemes:\n- type: apiKey\n  name: x-switch-key\n  evidence: '-H \"x-switch-key: $QP_KEY\"'\n  location: header\n  header: x-switch-key\n  how_to_obtain: Create API key in portal under Integraciones › Llaves de API › Crear llave, choose Prueba and copy the value.\ndocs: https://docs.pagaconquickpay.com/developers/quickstart.md\n"
source_yaml_url: https://artifacts.apis.io/pagaconquickpay-com/authentication/pagaconquickpay-com-authentication.yml
summary_line: 1 scheme
tags:
- Payments
- Fintech
- Venezuela
- WhatsApp
- QR
---
