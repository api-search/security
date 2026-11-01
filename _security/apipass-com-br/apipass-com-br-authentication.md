---
anonymous_access: false
api_key_in: []
api_specs:
- filename: apipass-com-br-openapi-generated.yml
  format: yaml
  label: Keila Santos API
  slug: apipass-com-br-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apipass-com-br/openapi/_ae-authored/apipass-com-br-openapi-generated.yml
auth_types: []
description: Authentication methods documented for the Apipass platform.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Apipass Com Br Authentication
name_suffix: Authentication
oauth_flows: []
overview: Keila Santos declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Keila Santos
provider_slug: apipass-com-br
scheme_count: 2
schemes:
- evidence: O *basic* é usado quando a requisição requer uma *basic auth*, ou atenticação basica, que é através de um usuário e uma senha, passando esses dados no basic a plataforma transforma isso em um *basic token* que é o mesmo que pegar um usuário e senha e converter em *base64*.
  header: Authorization
  how_to_obtain: Provide a username and password; the platform converts them to a Base64‑encoded token and places it in the Authorization header.
  location: header
  name: Basic Auth
  type: http-basic
- evidence: 'Por exemplo, se você estiver fazendo uma solicitação POST para uma API que requer autenticação via *header* "Authorization", você configuraria isso da seguinte maneira: * Chave (Key): Authorization * Valor (Value): Bearer <seu-token-de-autenticação>'
  header: Authorization
  how_to_obtain: Supply a JWT or other bearer token and set it as the value of the Authorization header prefixed with "Bearer ".
  location: header
  name: Bearer Token
  type: http-bearer
slug: apipass-com-br-authentication
source_filename: apipass-com-br-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.apipass.com.br/documentacao-apipass/configuracoes/mfa-multi-factor-authentication.md
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.apipass.com.br/documentacao-apipass/configuracoes/mfa-multi-factor-authentication.md\nsources:\n- https://docs.apipass.com.br/documentacao-apipass/configuracoes/mfa-multi-factor-authentication.md\n- https://docs.apipass.com.br/documentacao-apipass/triggers-and-conectores/conectores-steps/conector-http/query-params-headers-e-basic-auth.md\ndescription: Authentication methods documented for the Apipass platform.\nschemes:\n- type: http-basic\n  name: Basic Auth\n  evidence: O *basic* é usado quando a requisição requer uma *basic auth*, ou atenticação basica, que é através de um usuário e uma senha, passando\n    esses dados no basic a plataforma transforma isso em um *basic token* que é o mesmo que pegar um usuário e senha e converter em *base64*.\n  location: header\n  header: Authorization\n  how_to_obtain: Provide a username and password; the platform converts them\
  \ to a Base64‑encoded token and places it in the Authorization header.\n- type: http-bearer\n  name: Bearer Token\n  evidence: 'Por exemplo, se você estiver fazendo uma solicitação POST para uma API que requer autenticação via *header* \"Authorization\", você\n    configuraria isso da seguinte maneira: * Chave (Key): Authorization * Valor (Value): Bearer <seu-token-de-autenticação>'\n  location: header\n  header: Authorization\n  how_to_obtain: Supply a JWT or other bearer token and set it as the value of the Authorization header prefixed with \"Bearer \".\nnote: No OAuth2 flows, API key, or other authentication schemes were found on the provided pages.\ndocs: https://docs.apipass.com.br/documentacao-apipass/configuracoes/mfa-multi-factor-authentication.md\n"
source_yaml_url: https://artifacts.apis.io/apipass-com-br/authentication/apipass-com-br-authentication.yml
summary_line: 2 schemes
tags:
- Company
---
