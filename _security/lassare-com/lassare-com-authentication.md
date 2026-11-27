---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lassare-com-admin-api-openapi.yml
  format: yaml
  label: Lassare Admin API
  slug: lassare-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lassare-com/openapi/lassare-com-admin-api-openapi.yml
- filename: lassare-com-decision-api-openapi.yml
  format: yaml
  label: Lassare Decision API
  slug: lassare-com-decision-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lassare-com/openapi/lassare-com-decision-api-openapi.yml
- filename: lassare-com-health-api-openapi.yml
  format: yaml
  label: Lassare Health API
  slug: lassare-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lassare-com/openapi/lassare-com-health-api-openapi.yml
- filename: lassare-com-logs-api-openapi.yml
  format: yaml
  label: Lassare Logs API
  slug: lassare-com-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lassare-com/openapi/lassare-com-logs-api-openapi.yml
- filename: lassare-com-settings-api-openapi.yml
  format: yaml
  label: Lassare Settings API
  slug: lassare-com-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lassare-com/openapi/lassare-com-settings-api-openapi.yml
- filename: lassare-com-slack-api-openapi.yml
  format: yaml
  label: Lassare Slack API
  slug: lassare-com-slack-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lassare-com/openapi/lassare-com-slack-api-openapi.yml
- filename: lassare-com-teams-api-openapi.yml
  format: yaml
  label: Lassare Teams API
  slug: lassare-com-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lassare-com/openapi/lassare-com-teams-api-openapi.yml
- filename: lassare-com-webhook-decisions-api-openapi.yml
  format: yaml
  label: Lassare Webhook Decisions API
  slug: lassare-com-webhook-decisions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lassare-com/openapi/lassare-com-webhook-decisions-api-openapi.yml
auth_types: []
description: SSH key authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Lassare Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lassare declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Lassare
provider_slug: lassare-com
scheme_count: 1
schemes:
- evidence: When you connect via SSH, you authenticate using a private key file on your local machine.
  name: SSH key
  type: other
slug: lassare-com-authentication
source_filename: lassare-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.github.com/en/authentication/connecting-to-github-with-ssh
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.github.com/en/authentication/connecting-to-github-with-ssh\nsources:\n- https://docs.github.com/en/authentication/connecting-to-github-with-ssh\n- https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account\n- https://docs.github.com/en/authentication/connecting-to-github-with-ssh/checking-for-existing-ssh-keys\n- https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent\ndescription: SSH key authentication\nschemes:\n- type: other\n  name: SSH key\n  evidence: When you connect via SSH, you authenticate using a private key file on your local machine.\ndocs: https://docs.github.com/en/authentication/connecting-to-github-with-ssh\n"
source_yaml_url: https://artifacts.apis.io/lassare-com/authentication/lassare-com-authentication.yml
summary_line: 1 scheme
tags:
- Human-in-the-Loop
- MCP Protocol
- Remote agent control
- Developer Tools
---
