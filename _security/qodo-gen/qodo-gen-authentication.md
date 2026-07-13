---
api_key_in: []
api_specs:
- filename: qodo-gen-openapi.yml
  format: yaml
  label: Qodo Merge PR Review
  slug: qodo-gen-merge-pr-review-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qodo-gen/refs/heads/main/openapi/qodo-gen-openapi.yml
- filename: qodo-gen-openapi.yml
  format: yaml
  label: Qodo Merge Code Suggestions
  slug: qodo-gen-merge-code-suggestions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qodo-gen/refs/heads/main/openapi/qodo-gen-openapi.yml
- filename: qodo-gen-openapi.yml
  format: yaml
  label: Qodo Merge PR Description
  slug: qodo-gen-merge-describe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qodo-gen/refs/heads/main/openapi/qodo-gen-openapi.yml
- filename: qodo-gen-openapi.yml
  format: yaml
  label: Qodo Merge Ask and Chat
  slug: qodo-gen-merge-ask-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qodo-gen/refs/heads/main/openapi/qodo-gen-openapi.yml
- filename: qodo-gen-openapi.yml
  format: yaml
  label: Qodo Gen Test Generation
  slug: qodo-gen-test-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qodo-gen/refs/heads/main/openapi/qodo-gen-openapi.yml
- filename: qodo-gen-openapi.yml
  format: yaml
  label: Qodo Command Agent API
  slug: qodo-gen-command-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qodo-gen/refs/heads/main/openapi/qodo-gen-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Qodo Gen Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qodo secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Qodo
provider_slug: qodo-gen
scheme_count: 2
schemes:
- description: Qodo API key / token issued from the Qodo dashboard, used by the Qodo Command CLI and hosted platform surfaces. Enterprise supports BYOK (bring your own LLM keys). Exact header conventions are not publicly documented and are modeled.
  in: header
  keyName: Authorization
  name: qodoApiKey
  sources:
  - openapi/qodo-gen-openapi.yml
  type: apiKey
- description: Shared secret configured when installing the single-tenant Qodo Merge Git webhook, verified on each inbound event from the Git provider (GitHub / GitLab / Bitbucket / Azure DevOps).
  in: header
  keyName: X-Hub-Signature-256
  name: webhookSecret
  sources:
  - https://docs.qodo.ai/qodo-documentation/qodo-merge/getting-started/setup-and-installation/github/qodo-single-tenant-github
  type: apiKey
slug: qodo-gen-authentication
source_filename: qodo-gen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/qodo-gen-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: qodoApiKey\n  type: apiKey\n  in: header\n  keyName: Authorization\n  description: >-\n    Qodo API key / token issued from the Qodo dashboard, used by the Qodo Command\n    CLI and hosted platform surfaces. Enterprise supports BYOK (bring your own LLM\n    keys). Exact header conventions are not publicly documented and are modeled.\n  sources:\n  - openapi/qodo-gen-openapi.yml\n- name: webhookSecret\n  type: apiKey\n  in: header\n  keyName: X-Hub-Signature-256\n  description: >-\n    Shared secret configured when installing the single-tenant Qodo Merge Git\n    webhook, verified on each inbound event from the Git provider (GitHub / GitLab\n    / Bitbucket / Azure DevOps).\n  sources:\n  - https://docs.qodo.ai/qodo-documentation/qodo-merge/getting-started/setup-and-installation/github/qodo-single-tenant-github\nnotes: >-\n  Qodo does not publish\
  \ a documented public REST API with a formal auth scheme.\n  Qodo Merge (Git app) authenticates through the Git provider's app installation\n  and a webhook secret; the Qodo Command CLI authenticates to the Qodo platform\n  with an account token. Schemes above are derived/modeled, not lifted from a\n  vendor OpenAPI.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qodo-gen/refs/heads/main/authentication/qodo-gen-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- AI Coding Assistant
- Code Review
- Test Generation
- Developer Tools
- LLM
- AI
- Pull Request Review
- Code Quality
- Agents
- Open Source
---
