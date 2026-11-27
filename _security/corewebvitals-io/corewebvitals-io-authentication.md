---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: CoreWebVitals.io Authentication
name_suffix: Authentication
oauth_flows: []
overview: CoreWebVitals.io declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: CoreWebVitals.io
provider_slug: corewebvitals-io
scheme_count: 4
schemes:
- applies_to:
  - JSON-RPC data API at https://app.coredash.app/api/mcp
  - Uptime REST API
  description: Keys start with cdk_ and are scoped to a single project. Create one in app.coredash.app under the project, then AI Insights, then Connect Your AI. The key is shown only once. You can create multiple keys and revoke them from the same page.
  header: 'Authorization: Bearer cdk_YOUR_API_KEY'
  name: projectKey
  prefix: cdk_
  scheme: bearer
  scope: one project
  type: http
- applies_to:
  - Agency REST /api/agency/projects
  - JSON-RPC data API
  - Uptime REST API
  description: Master keys are only available on agency-flagged accounts. You mint them in the web UI under My Account, then the Agency API tab. The key is shown once and can be revoked from the same tab. A master key manages projects over REST and reads data for any project by passing project_id.
  header: 'Authorization: Bearer cdk_master_YOUR_MASTER_KEY'
  name: masterKey
  prefix: cdk_master_
  scheme: bearer
  scope: every project on the account
  type: http
- description: The OAuth token of an AI connection such as Claude (mcp_at_) is read-only. A POST, PATCH or DELETE made with it gets a 403.
  docs: https://www.coredash.app/api/uptime
  name: mcpOAuth
  token_prefix: mcp_at_
  type: oauth2
- applies_to:
  - https://www.corewebvitals.io/api/state-of-cwv/mcp
  description: The State of Web Vitals MCP is a free, no-auth remote MCP server.
  name: none
  type: none
slug: corewebvitals-io-authentication
source_filename: corewebvitals-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource:\n- https://www.coredash.app/api\n- https://www.coredash.app/api/agency\n- https://www.coredash.app/api/uptime\ndocs: https://www.coredash.app/api\nnote: No OpenAPI is published. This profile comes from the CoreDash docs pages. The State of Web Vitals MCP (https://www.corewebvitals.io/api/state-of-cwv/mcp) is documented as free and no-auth.\nschemes:\n- name: projectKey\n  type: http\n  scheme: bearer\n  header: 'Authorization: Bearer cdk_YOUR_API_KEY'\n  prefix: cdk_\n  scope: one project\n  description: Keys start with cdk_ and are scoped to a single project. Create one in app.coredash.app under the project, then AI Insights, then Connect Your AI. The key is shown only once. You can create multiple keys and revoke them from the same page.\n  applies_to: [JSON-RPC data API at https://app.coredash.app/api/mcp, Uptime REST API]\n- name: masterKey\n  type: http\n  scheme: bearer\n  header: 'Authorization: Bearer cdk_master_YOUR_MASTER_KEY'\n\
  \  prefix: cdk_master_\n  scope: every project on the account\n  description: Master keys are only available on agency-flagged accounts. You mint them in the web UI under My Account, then the Agency API tab. The key is shown once and can be revoked from the same tab. A master key manages projects over REST and reads data for any project by passing project_id.\n  applies_to: [Agency REST /api/agency/projects, JSON-RPC data API, Uptime REST API]\n- name: mcpOAuth\n  type: oauth2\n  token_prefix: mcp_at_\n  description: The OAuth token of an AI connection such as Claude (mcp_at_) is read-only. A POST, PATCH or DELETE made with it gets a 403.\n  docs: https://www.coredash.app/api/uptime\n- name: none\n  type: none\n  description: The State of Web Vitals MCP is a free, no-auth remote MCP server.\n  applies_to: [https://www.corewebvitals.io/api/state-of-cwv/mcp]\n"
source_yaml_url: https://artifacts.apis.io/corewebvitals-io/authentication/corewebvitals-io-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Core Web Vitals
- Web Performance
- Page Speed
- Real User Monitoring
- Consulting
- MCP
---
