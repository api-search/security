---
api_key_in:
- header
api_specs:
- filename: albacross-reveal-openapi.yml
  format: yaml
  label: Albacross Reveal API
  slug: albacross-reveal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/albacross/refs/heads/main/openapi/albacross-reveal-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Albacross Authentication
name_suffix: Authentication
oauth_flows: []
overview: Albacross secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Albacross
provider_slug: albacross
scheme_count: 1
schemes:
- applies_to:
  - Albacross Reveal API
  - Albacross Enrich API
  - Albacross n8n Automation API
  evidence:
  - sample: 'curl -X GET "https://api.albacross.com/reveal/company/192.0.2.1" -H "Authorization: Api-Key YOUR_API_KEY"'
    source: https://docs.albacross.com/reveal
  - sample: 'GET https://api.albacross.com/enrich/companies/example.com / Authorization: Api-Key YOUR_API_KEY'
    source: https://docs.albacross.com/enrich
  - sample: 'headers: { Authorization: ''=Api-Key {{$credentials.apiKey}}'' }'
    source: github.com/albacross/n8n-nodes-albacross credentials/AlbacrossApi.credentials.ts
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/albacross-reveal-openapi.yml
  - openapi/_original/albacross-reveal-openapi-original.yml
  type: apiKey
  value_format: Api-Key <YOUR_API_KEY>
slug: albacross-authentication
source_filename: albacross-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://docs.albacross.com/authentication\ndocs: https://docs.albacross.com/authentication\nderived_from:\n- openapi/albacross-reveal-openapi.yml\n- https://github.com/albacross/n8n-nodes-albacross/blob/main/credentials/AlbacrossApi.credentials.ts\n- live probes of api.albacross.com and reveal.api.albacross.com on 2026-08-12\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  oidc: false\n  mtls: false\n  scopes: false\nnote: >\n  One mechanism across the entire Albacross surface: a static, long-lived API key sent in the\n  Authorization header using a CUSTOM auth-scheme token, `Api-Key <key>`. This is not RFC 6750\n  Bearer and not RFC 7617 Basic. The published OpenAPI declares the scheme only as\n  `type: apiKey, in: header, name: Authorization` and OMITS the required `Api-Key ` prefix, so a\n  client generated from the spec alone will send the bare key and receive 401. The prefix is\n  visible only\
  \ in the documentation code samples and in Albacross's own MIT-licensed n8n\n  credential. This artifact is upgraded to `method: searched` specifically to record that prefix,\n  which the derived spec pass could not see.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  value_format: 'Api-Key <YOUR_API_KEY>'\n  sources:\n  - openapi/albacross-reveal-openapi.yml\n  - openapi/_original/albacross-reveal-openapi-original.yml\n  applies_to:\n  - Albacross Reveal API\n  - Albacross Enrich API\n  - Albacross n8n Automation API\n  evidence:\n  - {source: 'https://docs.albacross.com/reveal', sample: 'curl -X GET \"https://api.albacross.com/reveal/company/192.0.2.1\" -H \"Authorization: Api-Key YOUR_API_KEY\"'}\n  - {source: 'https://docs.albacross.com/enrich', sample: 'GET https://api.albacross.com/enrich/companies/example.com / Authorization: Api-Key YOUR_API_KEY'}\n  - {source: 'github.com/albacross/n8n-nodes-albacross credentials/AlbacrossApi.credentials.ts',\
  \ sample: \"headers: { Authorization: '=Api-Key {{$credentials.apiKey}}' }\"}\nkey_provisioning:\n  self_serve: false\n  entitlement: Organisation plan; \"API Access* — *Available upon request\"\n  channels:\n  - Account manager / sales (https://www.albacross.com/data-api states keys are provisioned through sales)\n  - 'Albacross dashboard, for the n8n key: Settings → Integrations → n8n'\n  note: >\n    A developer cannot obtain an Albacross API key without a sales conversation. There is no\n    self-serve key issuance, no developer signup that yields a key, and no sandbox key.\nkey_lifecycle:\n  rotation_documented: false\n  expiry: none\n  revocation_documented: false\n  multiple_keys: true\n  note: >\n    Keys are static and long-lived. No rotation policy, no expiry, no documented revocation flow\n    and no key-scoping. The n8n key is a separate named key, which implies per-integration keys are\n    possible, but no key-management documentation is published.\nscopes:\n  supported:\
  \ false\n  note: >\n    No OAuth, therefore no scopes. scopes/ is deliberately absent from this repo rather than\n    written empty. Coarse entitlement is enforced per key at the endpoint level — an anonymous or\n    unentitled call to Enrich returns 403 \"No authorization header\" while Reveal returns 401\n    \"Authentication required\", so entitlement differences do surface, inconsistently.\ncredential_transmission:\n  tls_required: true\n  observed_tls:\n  - {host: api.albacross.com, tls: TLSv1.2, hsts: false}\n  - {host: reveal.api.albacross.com, tls: TLSv1.2}\n  note: >\n    The API host negotiates TLS 1.2 and does not send HSTS, so a static long-lived bearer-style\n    credential travels to a host with no strict-transport guarantee. See\n    security/albacross-domain-security.yml.\nwebhook_authentication:\n  inbound_to_consumer: shared-token\n  signature: none\n  note: >\n    Outbound webhooks use an optional shared token, not an HMAC signature. See\n    asyncapi/albacross-webhooks.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/albacross/refs/heads/main/authentication/albacross-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- B2B Data
- Lead Generation
- Intent Data
- Company Enrichment
- IP Intelligence
- Firmographics
- Marketing
- Sales Intelligence
- Account Based Marketing
- Website Visitor Identification
- Webhook
---
