---
anonymous_access: false
api_key_in: []
api_specs:
- filename: contasimples-accounts-api-openapi.yml
  format: yaml
  label: Contasimples Accounts API
  slug: contasimples-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contasimples/refs/heads/main/openapi/contasimples-accounts-api-openapi.yml
- filename: contasimples-attachments-api-openapi.yml
  format: yaml
  label: Contasimples Attachments API
  slug: contasimples-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contasimples/refs/heads/main/openapi/contasimples-attachments-api-openapi.yml
- filename: contasimples-categories-api-openapi.yml
  format: yaml
  label: Contasimples Categories API
  slug: contasimples-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contasimples/refs/heads/main/openapi/contasimples-categories-api-openapi.yml
- filename: contasimples-cost-centers-api-openapi.yml
  format: yaml
  label: Contasimples Cost Centers API
  slug: contasimples-cost-centers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contasimples/refs/heads/main/openapi/contasimples-cost-centers-api-openapi.yml
- filename: contasimples-credit-cards-api-openapi.yml
  format: yaml
  label: Contasimples Credit Cards API
  slug: contasimples-credit-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contasimples/refs/heads/main/openapi/contasimples-credit-cards-api-openapi.yml
- filename: contasimples-oauth-api-openapi.yml
  format: yaml
  label: Contasimples OAuth API
  slug: contasimples-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contasimples/refs/heads/main/openapi/contasimples-oauth-api-openapi.yml
- filename: contasimples-statements-api-openapi.yml
  format: yaml
  label: Contasimples Statements API
  slug: contasimples-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contasimples/refs/heads/main/openapi/contasimples-statements-api-openapi.yml
- filename: contasimples-suppliers-api-openapi.yml
  format: yaml
  label: Contasimples Suppliers API
  slug: contasimples-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contasimples/refs/heads/main/openapi/contasimples-suppliers-api-openapi.yml
- filename: contasimples-users-api-openapi.yml
  format: yaml
  label: Contasimples Users API
  slug: contasimples-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contasimples/refs/heads/main/openapi/contasimples-users-api-openapi.yml
auth_types: []
description: OAuth 2.0 Client Credentials flow
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Contasimples Authentication
name_suffix: Authentication
oauth_flows: []
overview: Contasimples declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Contasimples
provider_slug: contasimples
scheme_count: 1
schemes:
- evidence: 'Obtém um token de acesso (JWT) via OAuth 2.0 Client Credentials. As credenciais api_key e api_secret devem ser enviadas no header Authorization: Basic , com o valor em base64 da string api_key:api_secret .'
  flows:
  - client_credentials
  header: Authorization
  how_to_obtain: 'Credenciais são gerenciadas no Internet Banking da Conta Simples; forneça api_key e api_secret codificados em base64 no cabeçalho Authorization: Basic.'
  location: header
  name: OAuth 2.0 Client Credentials
  token_url: https://api-sandbox.contasimples.com/oauth/v1/access-token
  type: oauth2
slug: contasimples-authentication
source_filename: contasimples-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.contasimples.com/br/api-reference/post-oauth-v1-access-token
source_yaml: "generated: '2026-10-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.contasimples.com/br/api-reference/post-oauth-v1-access-token\nsources:\n- https://developers.contasimples.com/br/api-reference/post-oauth-v1-access-token\n- https://developers.contasimples.com/en/api-reference/post-oauth-v1-access-token\n- https://developers.contasimples.com/br/comece-aqui/quickstart\n- https://developers.contasimples.com/en/comece-aqui/quickstart\ndescription: OAuth 2.0 Client Credentials flow\nschemes:\n- type: oauth2\n  name: OAuth 2.0 Client Credentials\n  evidence: 'Obtém um token de acesso (JWT) via OAuth 2.0 Client Credentials. As credenciais api_key e api_secret devem ser enviadas no header\n    Authorization: Basic , com o valor em base64 da string api_key:api_secret .'\n  location: header\n  header: Authorization\n  flows:\n  - client_credentials\n  token_url: https://api-sandbox.contasimples.com/oauth/v1/access-token\n  how_to_obtain:\
  \ 'Credenciais são gerenciadas no Internet Banking da Conta Simples; forneça api_key e api_secret codificados em base64 no cabeçalho\n    Authorization: Basic.'\ndocs: https://developers.contasimples.com/br/api-reference/post-oauth-v1-access-token\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contasimples/refs/heads/main/authentication/contasimples-authentication.yml
summary_line: 1 scheme
tags:
- Company
---
