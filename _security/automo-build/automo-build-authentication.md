---
anonymous_access: false
api_key_in: []
api_specs:
- filename: automo-build-agent-api-openapi.yml
  format: yaml
  label: Automo Agent API
  slug: automo-build-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/automo-build/openapi/automo-build-agent-api-openapi.yml
- filename: automo-build-mcp-api-openapi.yml
  format: yaml
  label: Automo MCP API
  slug: automo-build-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/automo-build/openapi/automo-build-mcp-api-openapi.yml
- filename: automo-build-oauth-api-openapi.yml
  format: yaml
  label: Automo OAuth API
  slug: automo-build-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/automo-build/openapi/automo-build-oauth-api-openapi.yml
- filename: automo-build-openapi-json-api-openapi.yml
  format: yaml
  label: Automo Openapi.json API
  slug: automo-build-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/automo-build/openapi/automo-build-openapi-json-api-openapi.yml
- filename: automo-build-well-known-api-openapi.yml
  format: yaml
  label: Automo .well Known API
  slug: automo-build-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/automo-build/openapi/automo-build-well-known-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Automo Build Authentication
name_suffix: Authentication
oauth_flows: []
overview: Automo declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Automo
provider_slug: automo-build
scheme_count: 1
schemes:
- description: Automo Build OAuth 2.1 authorization code with PKCE (S256)
  flows:
    authorizationCode:
      authorizationUrl: https://mcp.automo.build/oauth/authorize
      refreshUrl: https://mcp.automo.build/oauth/token
      tokenUrl: https://mcp.automo.build/oauth/token
  scopes:
  - description: List workspace memberships, whoami, switch the current workspace
    name: workspaces:read
  - description: List and search projects, project status, env var names, screenshots, deployment history
    name: projects:read
  - description: Create projects, wake sandboxes, share and clone links
    name: projects:write
  - description: Prompt a project's main agent
    name: prompts:write
  - description: Read any agent session the user can read in the app
    name: sessions:read
  - description: Open, continue and stop agent sessions (CTO, Doctor, Security, QA, Architect, builder spawns)
    name: sessions:write
  - description: 'The sign-off state of builder work: cards, verdicts, fixes, whose move it is'
    name: reviews:read
  - description: Promote, ask a reviewer, hand fixes to the builder, approve or cancel a review
    name: reviews:write
  - description: List playbooks and read their runs
    name: playbooks:read
  - description: Run a playbook
    name: playbooks:run
  - description: Create and edit playbooks
    name: playbooks:write
  - description: Pending publish, deployment status and history
    name: deployments:read
  - description: Propose and approve deployments, publish
    name: deployments:write
  - description: Read project chat history
    name: chat:read
  - description: Put a workspace on the Free plan
    name: billing:write
  type: oauth2
slug: automo-build-authentication
source_filename: automo-build-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: searched\nsource: https://automo.build/auth.md\nschemes:\n  - type: oauth2\n    description: \"Automo Build OAuth 2.1 authorization code with PKCE (S256)\"\n    flows:\n      authorizationCode:\n        authorizationUrl: https://mcp.automo.build/oauth/authorize\n        tokenUrl: https://mcp.automo.build/oauth/token\n        refreshUrl: https://mcp.automo.build/oauth/token\n    scopes:\n      - name: workspaces:read\n        description: \"List workspace memberships, whoami, switch the current workspace\"\n      - name: projects:read\n        description: \"List and search projects, project status, env var names, screenshots, deployment history\"\n      - name: projects:write\n        description: \"Create projects, wake sandboxes, share and clone links\"\n      - name: prompts:write\n        description: \"Prompt a project's main agent\"\n      - name: sessions:read\n        description: \"Read any agent session the user can read in the app\"\
  \n      - name: sessions:write\n        description: \"Open, continue and stop agent sessions (CTO, Doctor, Security, QA, Architect, builder spawns)\"\n      - name: reviews:read\n        description: \"The sign-off state of builder work: cards, verdicts, fixes, whose move it is\"\n      - name: reviews:write\n        description: \"Promote, ask a reviewer, hand fixes to the builder, approve or cancel a review\"\n      - name: playbooks:read\n        description: \"List playbooks and read their runs\"\n      - name: playbooks:run\n        description: \"Run a playbook\"\n      - name: playbooks:write\n        description: \"Create and edit playbooks\"\n      - name: deployments:read\n        description: \"Pending publish, deployment status and history\"\n      - name: deployments:write\n        description: \"Propose and approve deployments, publish\"\n      - name: chat:read\n        description: \"Read project chat history\"\n      - name: billing:write\n        description: \"Put a\
  \ workspace on the Free plan\"\n"
source_yaml_url: https://artifacts.apis.io/automo-build/authentication/automo-build-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Platform
- Low-Code
- Automation
- Software Development
---
