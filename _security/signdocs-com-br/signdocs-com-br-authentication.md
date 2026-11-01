---
anonymous_access: false
api_key_in: []
api_specs:
- filename: signdocs-com-br-authentication-api-openapi.yml
  format: yaml
  label: signdocs-com-br Authentication API
  slug: signdocs-com-br-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signdocs-com-br/openapi/signdocs-com-br-authentication-api-openapi.yml
- filename: signdocs-com-br-documents-api-openapi.yml
  format: yaml
  label: signdocs-com-br Documents API
  slug: signdocs-com-br-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signdocs-com-br/openapi/signdocs-com-br-documents-api-openapi.yml
- filename: signdocs-com-br-envelopes-api-openapi.yml
  format: yaml
  label: signdocs-com-br Envelopes API
  slug: signdocs-com-br-envelopes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signdocs-com-br/openapi/signdocs-com-br-envelopes-api-openapi.yml
- filename: signdocs-com-br-evidence-api-openapi.yml
  format: yaml
  label: signdocs-com-br Evidence API
  slug: signdocs-com-br-evidence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signdocs-com-br/openapi/signdocs-com-br-evidence-api-openapi.yml
- filename: signdocs-com-br-health-api-openapi.yml
  format: yaml
  label: signdocs-com-br Health API
  slug: signdocs-com-br-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signdocs-com-br/openapi/signdocs-com-br-health-api-openapi.yml
- filename: signdocs-com-br-signing-api-openapi.yml
  format: yaml
  label: signdocs-com-br Signing API
  slug: signdocs-com-br-signing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signdocs-com-br/openapi/signdocs-com-br-signing-api-openapi.yml
- filename: signdocs-com-br-signingsessions-api-openapi.yml
  format: yaml
  label: signdocs-com-br Signing Sessions API
  slug: signdocs-com-br-signingsessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signdocs-com-br/openapi/signdocs-com-br-signingsessions-api-openapi.yml
- filename: signdocs-com-br-steps-api-openapi.yml
  format: yaml
  label: signdocs-com-br Steps API
  slug: signdocs-com-br-steps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signdocs-com-br/openapi/signdocs-com-br-steps-api-openapi.yml
- filename: signdocs-com-br-transactions-api-openapi.yml
  format: yaml
  label: signdocs-com-br Transactions API
  slug: signdocs-com-br-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signdocs-com-br/openapi/signdocs-com-br-transactions-api-openapi.yml
- filename: signdocs-com-br-trustsessions-api-openapi.yml
  format: yaml
  label: signdocs-com-br Trust Sessions API
  slug: signdocs-com-br-trustsessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signdocs-com-br/openapi/signdocs-com-br-trustsessions-api-openapi.yml
- filename: signdocs-com-br-users-api-openapi.yml
  format: yaml
  label: signdocs-com-br Users API
  slug: signdocs-com-br-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signdocs-com-br/openapi/signdocs-com-br-users-api-openapi.yml
- filename: signdocs-com-br-verification-api-openapi.yml
  format: yaml
  label: signdocs-com-br Verification API
  slug: signdocs-com-br-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signdocs-com-br/openapi/signdocs-com-br-verification-api-openapi.yml
- filename: signdocs-com-br-webhooks-api-openapi.yml
  format: yaml
  label: signdocs-com-br Webhooks API
  slug: signdocs-com-br-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signdocs-com-br/openapi/signdocs-com-br-webhooks-api-openapi.yml
- filename: signdocs-com-br-document-groups-api-openapi.yml
  format: yaml
  label: signdocs-com-br Document Groups API
  slug: signdocs-com-br-document-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/signdocs-com-br/openapi/signdocs-com-br-document-groups-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Signdocs Com Br Authentication
name_suffix: Authentication
oauth_flows: []
overview: signdocs-com-br declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: signdocs-com-br
provider_slug: signdocs-com-br
scheme_count: 2
schemes:
- evidence: Autentique com OAuth2 client_credentials em POST /oauth2/token .
  flows:
  - client_credentials
  how_to_obtain: Use client_id and client_secret to request an access_token via POST to the token URL.
  name: OAuth2
  scopes:
  - transactions:read
  - transactions:write
  - steps:write
  - evidence:read
  - webhooks:write
  - verification:write
  token_url: https://api-hml.signdocs.com.br/oauth2/token
  type: oauth2
- evidence: O clientSecret é a autenticação daquela sessão e precisa viajar junto, no parâmetro cs .
  how_to_obtain: Returned once in the response of POST /v1/signing-sessions and used as the cs query parameter.
  location: query
  name: session clientSecret
  type: other
slug: signdocs-com-br-authentication
source_filename: signdocs-com-br-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.signdocs.com.br/guias/assinatura-expressa.html
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.signdocs.com.br/guias/assinatura-expressa.html\nsources:\n- https://docs.signdocs.com.br/guias/assinatura-expressa.html\n- https://docs.signdocs.com.br/guias/solucao-fornecedores.html\nschemes:\n- type: oauth2\n  name: OAuth2\n  evidence: Autentique com OAuth2 client_credentials em POST /oauth2/token .\n  flows:\n  - client_credentials\n  token_url: https://api-hml.signdocs.com.br/oauth2/token\n  scopes:\n  - transactions:read\n  - transactions:write\n  - steps:write\n  - evidence:read\n  - webhooks:write\n  - verification:write\n  how_to_obtain: Use client_id and client_secret to request an access_token via POST to the token URL.\n- type: other\n  name: session clientSecret\n  evidence: O clientSecret é a autenticação daquela sessão e precisa viajar junto, no parâmetro cs .\n  location: query\n  how_to_obtain: Returned once in the response of POST /v1/signing-sessions\
  \ and used as the cs query parameter.\ndocs: https://docs.signdocs.com.br/guias/assinatura-expressa.html\n"
source_yaml_url: https://artifacts.apis.io/signdocs-com-br/authentication/signdocs-com-br-authentication.yml
summary_line: 2 schemes
tags:
- Company
- DigitalSignature
- Brazil
- API
- DocumentManagement
---
