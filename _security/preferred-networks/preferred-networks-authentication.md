---
api_key_in: []
auth_types: []
description: Authentication profile for the PLaMo API, read from the provider's quickstart, console manual and API reference. There is no published OpenAPI to derive securitySchemes from, so every field below comes from the documentation text and from an unauthenticated probe of the API host.
kind: authentication
layout: security
method: searched
name: Preferred Networks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Preferred Networks declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Preferred Networks
provider_slug: preferred-networks
scheme_count: 1
schemes:
- description: A PLaMo API key issued from the PLaMo API console. The key is presented as an HTTP bearer token. Because the interface is OpenAI-compatible, OpenAI/LangChain client libraries authenticate by reading OPENAI_API_KEY while curl examples read PLAMO_API_KEY; both carry the same PLaMo key.
  environment_variable: PLAMO_API_KEY (OPENAI_API_KEY when using openai / langchain-openai)
  format: 'Authorization: Bearer ${PLAMO_API_KEY}'
  header: Authorization
  in: header
  key_prefix: not documented
  name: plamo_api_key
  scheme: bearer
  type: http
slug: preferred-networks-authentication
source_filename: preferred-networks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://docs.plamo.preferredai.jp/en/getting-started\nname: Preferred Networks PLaMo API authentication\ndescription: >-\n  Authentication profile for the PLaMo API, read from the provider's quickstart, console manual and\n  API reference. There is no published OpenAPI to derive securitySchemes from, so every field below\n  comes from the documentation text and from an unauthenticated probe of the API host.\ndocs:\n- https://docs.plamo.preferredai.jp/en/getting-started\n- https://docs.plamo.preferredai.jp/en/console\n- https://docs.plamo.preferredai.jp/en/api\nschemes:\n- name: plamo_api_key\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer ${PLAMO_API_KEY}'\n  description: >-\n    A PLaMo API key issued from the PLaMo API console. The key is presented as an HTTP bearer token.\n    Because the interface is OpenAI-compatible, OpenAI/LangChain client libraries authenticate\
  \ by\n    reading OPENAI_API_KEY while curl examples read PLAMO_API_KEY; both carry the same PLaMo key.\n  key_prefix: not documented\n  environment_variable: PLAMO_API_KEY (OPENAI_API_KEY when using openai / langchain-openai)\noauth2: false\nopenid_connect: false\nmutual_tls: false\nsigned_requests: false\nkey_model:\n  tenancy:\n    tenant: >-\n      Top-level management and billing unit. One tenant per PLaMo API billing account; usage across\n      all of its projects is aggregated and billed together.\n    project: >-\n      Unit for managing API keys and budgets inside a tenant. A default project named \"Default\"\n      exists initially and all tenant members belong to it.\n  key_types:\n  - name: Personal API key\n    scope: One per member, created from the profile page\n    revocation: Immediately invalidated when the member is removed from the tenant\n    accounting: Usage counts only toward the tenant total, not toward a project\n  - name: Project API key\n    scope: Multiple\
  \ per project, created by a project administrator\n    revocation: Survives removal of project members\n    accounting: Usage counts toward both the project and the tenant total\n  rotation:\n    supported: true\n    mechanism: Re-generate or delete a key from the console\n    semantics: >-\n      Re-generating a key invalidates the old key immediately, with no overlap window; PFN's own\n      guidance is to create a second key and cut traffic over before re-generating.\nroles:\n- name: Tenant Administrator\n  grants: All projects and resources; create/delete projects, set usage limits and alerts, invite and remove tenant members, manage permissions\n- name: Project Administrator\n  grants: Create, delete and re-generate API keys in their projects; add/remove project members (must already be tenant members); view project usage and spend\n- name: Member\n  grants: View usage and spend for projects they belong to; cannot create, delete or re-generate API keys\ninvitation_flow: >-\n  A tenant\
  \ administrator invites a user as either Tenant Administrator or Regular User; after the\n  invitation is accepted, a tenant or project administrator adds them to a project.\nanonymous_probe:\n  url: https://api.platform.preferredai.jp/v1/models\n  status: 400\n  body: '{\"message\":\"missing key in request header\"}'\n  note: >-\n    The API rejects a keyless request with HTTP 400 and a plain message envelope rather than 401 with\n    a WWW-Authenticate challenge, so there is no machine-discoverable auth challenge on this API.\nconsole: https://console.platform.preferredai.jp/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/preferred-networks/refs/heads/main/authentication/preferred-networks-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Machine-Learning
- Large Language Models
- Generative AI
- LLM Inference
- Foundation Models
- Japan
- Semiconductors
- Supercomputing
- Translation
- MCP
---
