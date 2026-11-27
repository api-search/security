---
anonymous_access: true
api_key_in: []
api_specs:
- filename: casanest-eu-public-api-openapi.yml
  format: yaml
  label: CasaNest Public API
  slug: casanest-eu-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/casanest-eu/openapi/casanest-eu-public-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: CasaNest Authentication
name_suffix: Authentication
oauth_flows: []
overview: CasaNest declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: CasaNest
provider_slug: casanest-eu
scheme_count: 3
schemes:
- api: CasaNest Public Catalogue API
  applies_to:
  - https://casanest.eu/api/public/v1
  - https://casanest.eu/mcp
  evidence: 'Autenticação: nenhuma; apenas imóveis que já estão publicados no portal.'
  name: none (public catalogue API and MCP)
  source: https://casanest.eu/casanest-ai.md
  type: none
- alternate: While logged in to the Provider dashboard, the same routes also answer (session).
  api: CasaNest CRM Partner API
  applies_to:
  - https://casanest.eu/api/parceiro/v1
  evidence: 'Send it with every request in the Authorization: users API-Key <key> header (this exact form, no Bearer ).'
  format: 'Authorization: users API-Key <key>'
  header: Authorization
  in: header
  issuance: Generated under Your CRM → API key; shown once; generating a new key disables the previous one immediately.
  key_prefix_example: cnp_
  name: Partner API key
  restrictions: Only works for CRM provider accounts; reads reports and manages pre-approved agencies; cannot create keys or change the webhook.
  source: https://casanest.eu/en/crm/documentation
  type: apiKey
- algorithm: HMAC-SHA256 over "${t}.${body}" keyed with the signing secret
  direction: outbound-webhook
  format: t=<unix>,sha256=<hex>
  header: X-CasaNest-Assinatura
  name: Webhook HMAC signature
  replay_tolerance: reject if t is more than 5 minutes from your clock
  source: https://casanest.eu/en/crm/documentation
  type: hmac-signature
slug: casanest-eu-authentication
source_filename: casanest-eu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://casanest.eu/en/crm/documentation\ndocs: https://casanest.eu/en/crm/documentation\nnote: The public OpenAPI (openapi/casanest-eu-openapi.yml) declares no securitySchemes and an empty security list; the technical guide states the public catalogue and MCP server need no authentication. The CRM Partner API is documented in HTML only.\nschemes:\n- name: none (public catalogue API and MCP)\n  type: none\n  api: CasaNest Public Catalogue API\n  applies_to:\n  - https://casanest.eu/api/public/v1\n  - https://casanest.eu/mcp\n  evidence: \"Autenticação: nenhuma; apenas imóveis que já estão publicados no portal.\"\n  source: https://casanest.eu/casanest-ai.md\n- name: Partner API key\n  type: apiKey\n  in: header\n  header: Authorization\n  format: 'Authorization: users API-Key <key>'\n  api: CasaNest CRM Partner API\n  applies_to:\n  - https://casanest.eu/api/parceiro/v1\n  key_prefix_example: cnp_\n  evidence: \"Send it with\
  \ every request in the Authorization: users API-Key <key> header (this exact form, no Bearer ).\"\n  issuance: Generated under Your CRM → API key; shown once; generating a new key disables the previous one immediately.\n  restrictions: Only works for CRM provider accounts; reads reports and manages pre-approved agencies; cannot create keys or change the webhook.\n  alternate: While logged in to the Provider dashboard, the same routes also answer (session).\n  source: https://casanest.eu/en/crm/documentation\n- name: Webhook HMAC signature\n  type: hmac-signature\n  direction: outbound-webhook\n  header: X-CasaNest-Assinatura\n  format: t=<unix>,sha256=<hex>\n  algorithm: HMAC-SHA256 over \"${t}.${body}\" keyed with the signing secret\n  replay_tolerance: reject if t is more than 5 minutes from your clock\n  source: https://casanest.eu/en/crm/documentation\n"
source_yaml_url: https://artifacts.apis.io/casanest-eu/authentication/casanest-eu-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Real Estate
- Property Listings
- Portugal
- PropTech
- CRM Integration
- MCP
- Housing Statistics
---
