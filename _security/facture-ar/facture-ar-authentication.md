---
anonymous_access: false
api_key_in: []
api_specs:
- filename: facture-ar-borradores-api-openapi.yml
  format: yaml
  label: Facturear Borradores API
  slug: facture-ar-borradores-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/facture-ar/openapi/facture-ar-borradores-api-openapi.yml
- filename: facture-ar-cuits-api-openapi.yml
  format: yaml
  label: Facturear CUITs API
  slug: facture-ar-cuits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/facture-ar/openapi/facture-ar-cuits-api-openapi.yml
- filename: facture-ar-facturas-api-openapi.yml
  format: yaml
  label: Facturear Facturas API
  slug: facture-ar-facturas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/facture-ar/openapi/facture-ar-facturas-api-openapi.yml
- filename: facture-ar-importar-desde-arca-api-openapi.yml
  format: yaml
  label: Facturear Importar desde ARCA API
  slug: facture-ar-importar-desde-arca-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/facture-ar/openapi/facture-ar-importar-desde-arca-api-openapi.yml
- filename: facture-ar-lotes-api-openapi.yml
  format: yaml
  label: Facturear Lotes API
  slug: facture-ar-lotes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/facture-ar/openapi/facture-ar-lotes-api-openapi.yml
- filename: facture-ar-plantillas-api-openapi.yml
  format: yaml
  label: Facturear Plantillas API
  slug: facture-ar-plantillas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/facture-ar/openapi/facture-ar-plantillas-api-openapi.yml
- filename: facture-ar-reportes-api-openapi.yml
  format: yaml
  label: Facturear Reportes API
  slug: facture-ar-reportes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/facture-ar/openapi/facture-ar-reportes-api-openapi.yml
- filename: facture-ar-utilidades-api-openapi.yml
  format: yaml
  label: Facturear Utilidades API
  slug: facture-ar-utilidades-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/facture-ar/openapi/facture-ar-utilidades-api-openapi.yml
- filename: facture-ar-webhooks-api-openapi.yml
  format: yaml
  label: Facturear Webhooks API
  slug: facture-ar-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/facture-ar/openapi/facture-ar-webhooks-api-openapi.yml
auth_types: []
description: API Key authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Facturear Authentication
name_suffix: Authentication
oauth_flows: []
overview: Facturear declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Facturear
provider_slug: facture-ar
scheme_count: 1
schemes:
- evidence: La API Key es el mecanismo de autenticación principal de la API de Facturear. Toda llamada a la API debe incluir una API Key válida en el header x-api-key .
  header: x-api-key
  how_to_obtain: Se generan desde el dashboard de Facturear, una para producción (prefijo prod_sk_) y otra para testing (prefijo test_sk_).
  location: header
  name: API Key
  type: apiKey
slug: facture-ar-authentication
source_filename: facture-ar-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.facture.ar/es/guides/api-keys
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.facture.ar/es/guides/api-keys\nsources:\n- https://docs.facture.ar/es/guides/api-keys\n- https://docs.facture.ar/es/getting-started/index\ndescription: API Key authentication\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: La API Key es el mecanismo de autenticación principal de la API de Facturear. Toda llamada a la API debe incluir una API Key válida\n    en el header x-api-key .\n  location: header\n  header: x-api-key\n  how_to_obtain: Se generan desde el dashboard de Facturear, una para producción (prefijo prod_sk_) y otra para testing (prefijo test_sk_).\ndocs: https://docs.facture.ar/es/guides/api-keys\n"
source_yaml_url: https://artifacts.apis.io/facture-ar/authentication/facture-ar-authentication.yml
summary_line: 1 scheme
tags:
- Billing
- Invoicing
- Argentina
- Software-as-a-Service
---
