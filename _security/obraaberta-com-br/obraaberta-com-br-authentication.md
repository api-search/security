---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: obraaberta-com-br-construtoras-api-openapi.yml
  format: yaml
  label: ObraAberta Construtoras API
  slug: obraaberta-com-br-construtoras-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obraaberta-com-br/openapi/obraaberta-com-br-construtoras-api-openapi.yml
- filename: obraaberta-com-br-dados-api-openapi.yml
  format: yaml
  label: ObraAberta Dados API
  slug: obraaberta-com-br-dados-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obraaberta-com-br/openapi/obraaberta-com-br-dados-api-openapi.yml
- filename: obraaberta-com-br-metabuscador-api-openapi.yml
  format: yaml
  label: ObraAberta Metabuscador API
  slug: obraaberta-com-br-metabuscador-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obraaberta-com-br/openapi/obraaberta-com-br-metabuscador-api-openapi.yml
- filename: obraaberta-com-br-partner-api-api-openapi.yml
  format: yaml
  label: ObraAberta Partner API
  slug: obraaberta-com-br-partner-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obraaberta-com-br/openapi/obraaberta-com-br-partner-api-api-openapi.yml
- filename: obraaberta-com-br-projetos-api-openapi.yml
  format: yaml
  label: ObraAberta Projetos API
  slug: obraaberta-com-br-projetos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obraaberta-com-br/openapi/obraaberta-com-br-projetos-api-openapi.yml
- filename: obraaberta-com-br-sistema-api-openapi.yml
  format: yaml
  label: ObraAberta Sistema API
  slug: obraaberta-com-br-sistema-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obraaberta-com-br/openapi/obraaberta-com-br-sistema-api-openapi.yml
- filename: obraaberta-com-br-transpar-ncia-condominial-api-openapi.yml
  format: yaml
  label: ObraAberta Transparência condominial API
  slug: obraaberta-com-br-transpar-ncia-condominial-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obraaberta-com-br/openapi/obraaberta-com-br-transpar-ncia-condominial-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 5
method: derived
name: ObraAberta Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: ObraAberta secures its APIs with apiKey, http, and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: ObraAberta
provider_slug: obraaberta-com-br
scheme_count: 5
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/obraaberta-com-br-openapi.yml
  type: http
- in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/obraaberta-com-br-openapi.yml
  type: apiKey
- description: Chave privada do condomínio. Guarde somente no servidor integrador.
  in: header
  name: condominiumApiKey
  parameter: X-ObraAberta-Key
  sources:
  - openapi/obraaberta-com-br-openapi.yml
  type: apiKey
- description: Chave secreta do conector de catálogo. É exibida uma única vez e deve permanecer somente no servidor do parceiro.
  in: header
  name: connectorApiKey
  parameter: X-ObraAberta-Connector-Key
  sources:
  - openapi/obraaberta-com-br-openapi.yml
  type: apiKey
- description: OAuth 2.0 Client Credentials para a Partner API sandbox.
  flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://obraaberta.com.br/api/v1/partners/oauth/token
  name: partnerOAuth2
  sources:
  - openapi/obraaberta-com-br-openapi.yml
  type: oauth2
slug: obraaberta-com-br-authentication
source_filename: obraaberta-com-br-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/obraaberta-com-br-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/obraaberta-com-br-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/obraaberta-com-br-openapi.yml\n- name: condominiumApiKey\n  type: apiKey\n  in: header\n  parameter: X-ObraAberta-Key\n  description: Chave privada do condomínio. Guarde somente no servidor integrador.\n  sources:\n  - openapi/obraaberta-com-br-openapi.yml\n- name: connectorApiKey\n  type: apiKey\n  in: header\n  parameter: X-ObraAberta-Connector-Key\n  description: Chave secreta do conector de catálogo. É exibida uma única vez e deve permanecer\n    somente no servidor do parceiro.\n  sources:\n  - openapi/obraaberta-com-br-openapi.yml\n-\
  \ name: partnerOAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://obraaberta.com.br/api/v1/partners/oauth/token\n    scopes: 2\n  description: OAuth 2.0 Client Credentials para a Partner API sandbox.\n  sources:\n  - openapi/obraaberta-com-br-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/obraaberta-com-br/authentication/obraaberta-com-br-authentication.yml
summary_line: apiKey/http/oauth2 · 5 schemes
tags:
- Construction
- Transparency
- Brazil
- Real Estate
- Public Data
---
