---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mcpdoafiliado-com-openapi-generated.yml
  format: yaml
  label: MCP do Afiliado API
  slug: mcpdoafiliado-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcpdoafiliado-com/openapi/_ae-authored/mcpdoafiliado-com-openapi-generated.yml
auth_types: []
description: Authentication methods for MCP do Afiliado
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: MCP do Afiliado Authentication
name_suffix: Authentication
oauth_flows: []
overview: MCP do Afiliado declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: MCP do Afiliado
provider_slug: mcpdoafiliado-com
scheme_count: 2
schemes:
- evidence: Como manda o próprio app cuida do token header X-API-Key
  header: X-API-Key
  how_to_obtain: Generate in the panel under Conectar IA; the full key appears once at creation.
  location: header
  name: X-API-Key
  type: apiKey
- evidence: Nos apps web você cola a URL do servidor, o app se registra sozinho (DCR), você entra com a sua conta e aprova a tela de consentimento.
  how_to_obtain: App registers via DCR in the panel, user logs in and approves consent screen; tokens are renewed automatically.
  name: OAuth 2.1
  type: oauth2
slug: mcpdoafiliado-com-authentication
source_filename: mcpdoafiliado-com-authentication.yml
source_heading: Authentication Profile
source_url: https://mcpdoafiliado.com/docs/autenticacao
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mcpdoafiliado.com/docs/autenticacao\nsources:\n- https://mcpdoafiliado.com/docs/autenticacao\ndescription: Authentication methods for MCP do Afiliado\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: Como manda o próprio app cuida do token header X-API-Key\n  location: header\n  header: X-API-Key\n  how_to_obtain: Generate in the panel under Conectar IA; the full key appears once at creation.\n- type: oauth2\n  name: OAuth 2.1\n  evidence: Nos apps web você cola a URL do servidor, o app se registra sozinho (DCR), você entra com a sua conta e aprova a tela de consentimento.\n  how_to_obtain: App registers via DCR in the panel, user logs in and approves consent screen; tokens are renewed automatically.\ndocs: https://mcpdoafiliado.com/docs/autenticacao\n"
source_yaml_url: https://artifacts.apis.io/mcpdoafiliado-com/authentication/mcpdoafiliado-com-authentication.yml
summary_line: 2 schemes
tags:
- Affiliates
- Artificial Intelligence
- E-Commerce
- Marketing
- Free
---
