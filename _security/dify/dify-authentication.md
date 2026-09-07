---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dify-service-api-openapi.json
  format: json
  label: Dify
  slug: dify
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/_original/dify-service-api-openapi.json
- filename: dify-chat-api-openapi.yml
  format: yaml
  label: Dify Chat Messages API
  slug: dify-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-chat-api-openapi.yml
- filename: dify-completion-api-openapi.yml
  format: yaml
  label: Dify Completion Messages API
  slug: dify-completion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-completion-api-openapi.yml
- filename: dify-conversations-api-openapi.yml
  format: yaml
  label: Dify Conversations API
  slug: dify-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-conversations-api-openapi.yml
- filename: dify-datasets-api-openapi.yml
  format: yaml
  label: Dify Knowledge Bases API
  slug: dify-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-datasets-api-openapi.yml
- filename: dify-files-api-openapi.yml
  format: yaml
  label: Dify Files API
  slug: dify-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-files-api-openapi.yml
- filename: dify-workflows-api-openapi.yml
  format: yaml
  label: Dify Workflow Runs API
  slug: dify-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-workflows-api-openapi.yml
- filename: dify-applications-api-openapi.yml
  format: yaml
  label: Dify Applications API
  slug: dify-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-applications-api-openapi.yml
- filename: dify-annotations-api-openapi.yml
  format: yaml
  label: Dify Annotations API
  slug: dify-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-annotations-api-openapi.yml
- filename: dify-audio-api-openapi.yml
  format: yaml
  label: Dify Audio API
  slug: dify-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-audio-api-openapi.yml
- filename: dify-feedback-api-openapi.yml
  format: yaml
  label: Dify Feedback API
  slug: dify-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-feedback-api-openapi.yml
- filename: dify-end-users-api-openapi.yml
  format: yaml
  label: Dify End Users API
  slug: dify-end-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-end-users-api-openapi.yml
- filename: dify-human-input-api-openapi.yml
  format: yaml
  label: Dify Human Input API
  slug: dify-human-input-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-human-input-api-openapi.yml
- filename: dify-documents-api-openapi.yml
  format: yaml
  label: Dify Documents API
  slug: dify-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-documents-api-openapi.yml
- filename: dify-chunks-api-openapi.yml
  format: yaml
  label: Dify Chunks API
  slug: dify-chunks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-chunks-api-openapi.yml
- filename: dify-tags-api-openapi.yml
  format: yaml
  label: Dify Knowledge Tags API
  slug: dify-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-tags-api-openapi.yml
- filename: dify-metadata-api-openapi.yml
  format: yaml
  label: Dify Metadata API
  slug: dify-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-metadata-api-openapi.yml
- filename: dify-models-api-openapi.yml
  format: yaml
  label: Dify Models API
  slug: dify-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-models-api-openapi.yml
- filename: dify-knowledge-pipeline-api-openapi.yml
  format: yaml
  label: Dify Knowledge Pipeline API
  slug: dify-knowledge-pipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-knowledge-pipeline-api-openapi.yml
auth_types:
- http
description: Dify authenticates every Service API request with a bearer API key. There is exactly one securityScheme across all 82 operations, but two distinct key FAMILIES flow through it, with very different blast radii — a fact the spec states in prose and the scheme itself cannot express.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Dify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dify secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dify
provider_slug: dify
scheme_count: 1
schemes:
- bearerFormat: API_KEY
  description: 'Every request authenticates with an API key: `Authorization: Bearer {API_KEY}`. App endpoints take an app API key; knowledge endpoints take a knowledge base API key ([Get Started](/en/api-reference/guides/get-started)).


    Keep keys server-side; never embed them in client code. Requests with a missing or invalid key fail with HTTP `401` (`unauthorized`).'
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/dify-annotations-api-openapi.yml
  - openapi/dify-applications-api-openapi.yml
  - openapi/dify-audio-api-openapi.yml
  - openapi/dify-chat-api-openapi.yml
  - openapi/dify-chunks-api-openapi.yml
  - openapi/dify-completion-api-openapi.yml
  - openapi/dify-conversations-api-openapi.yml
  - openapi/dify-datasets-api-openapi.yml
  - openapi/dify-documents-api-openapi.yml
  - openapi/dify-end-users-api-openapi.yml
  - openapi/dify-feedback-api-openapi.yml
  - openapi/dify-files-api-openapi.yml
  - openapi/dify-human-input-api-openapi.yml
  - openapi/dify-knowledge-pipeline-api-openapi.yml
  - openapi/dify-metadata-api-openapi.yml
  - openapi/dify-models-api-openapi.yml
  - openapi/dify-tags-api-openapi.yml
  - openapi/dify-workflows-api-openapi.yml
  type: http
slug: dify-authentication
source_filename: dify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://docs.dify.ai/en/api-reference/guides/get-started + openapi/_original/dify-service-api-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API_KEY\n  description: 'Every request authenticates with an API key: `Authorization: Bearer {API_KEY}`. App endpoints\n    take an app API key; knowledge endpoints take a knowledge base API key ([Get Started](/en/api-reference/guides/get-started)).\n\n\n    Keep keys server-side; never embed them in client code. Requests with a missing or invalid key fail\n    with HTTP `401` (`unauthorized`).'\n  sources:\n  - openapi/dify-annotations-api-openapi.yml\n  - openapi/dify-applications-api-openapi.yml\n  - openapi/dify-audio-api-openapi.yml\n  - openapi/dify-chat-api-openapi.yml\n  - openapi/dify-chunks-api-openapi.yml\n  - openapi/dify-completion-api-openapi.yml\n  - openapi/dify-conversations-api-openapi.yml\n  -\
  \ openapi/dify-datasets-api-openapi.yml\n  - openapi/dify-documents-api-openapi.yml\n  - openapi/dify-end-users-api-openapi.yml\n  - openapi/dify-feedback-api-openapi.yml\n  - openapi/dify-files-api-openapi.yml\n  - openapi/dify-human-input-api-openapi.yml\n  - openapi/dify-knowledge-pipeline-api-openapi.yml\n  - openapi/dify-metadata-api-openapi.yml\n  - openapi/dify-models-api-openapi.yml\n  - openapi/dify-tags-api-openapi.yml\n  - openapi/dify-workflows-api-openapi.yml\ndocs: https://docs.dify.ai/en/api-reference/guides/get-started\ndescription: Dify authenticates every Service API request with a bearer API key. There is exactly one\n  securityScheme across all 82 operations, but two distinct key FAMILIES flow through it, with very different\n  blast radii — a fact the spec states in prose and the scheme itself cannot express.\nkey_families:\n- name: app API key\n  scope: one published app; one key serves all of that app's end users\n  minted: inside the app in the Dify console\n  used_by:\
  \ chat messages, completion messages, workflow runs, conversations, files, audio, annotations,\n    feedback, applications, end users, human input\n- name: knowledge base API key\n  scope: every knowledge base visible to the account that created the key\n  minted: Knowledge -> Service API in the Dify console\n  used_by: knowledge bases, documents, chunks, metadata, tags, models, knowledge pipeline\n  caution: Broader than an app key. Dify's own spec description flags it as a data-security concern; there\n    is no per-knowledge-base scoping.\ntransport:\n  header: Authorization\n  format: Bearer {API_KEY}\n  scheme: bearer\n  bearerFormat: API_KEY\nfailure:\n  status: 401\n  code: unauthorized\n  note: Missing or invalid key.\nguidance:\n- Call the API from a backend only; a key in frontend code can be extracted.\n- Rotate by minting a new key in the console; no rotation endpoint exists in the API.\noauth2:\n  present: false\n  note: No oauth2 or openIdConnect securityScheme, and no OAuth\
  \ discovery document on any Dify host. SSO\n    exists on the Enterprise tier but is a console feature, not an API auth mode.\nscopes:\n  present: false\n  note: Key-auth only; there is no scope surface, so no scopes/ artifact is written.\nmtls:\n  present: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/authentication/dify-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- LLMOps
- Backend-as-a-Service
- Agents
- Workflows
- Knowledge Management
- RAG
- Model Context Protocol
- Low Code
- Open Source
---
