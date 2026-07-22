---
api_key_in: []
auth_types:
- snowflake-connection
description: ''
kind: authentication
layout: security
method: searched
name: Relationalai Authentication
name_suffix: Authentication
oauth_flows: []
overview: RelationalAI secures its APIs with snowflake-connection across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RelationalAI
provider_slug: relationalai
scheme_count: 1
schemes:
- granted_via: Snowflake RBAC roles (e.g. rai_developer)
  mechanism: Snowflake connection profile (key-pair / SSO / password)
  name: SnowflakeConnection
  notes: Configured via the SDK/CLI connection profile; the RelationalAI Native App must be installed in the Snowflake account and the calling user granted the appropriate RelationalAI role.
  sources:
  - https://docs.relational.ai/build/setup
  type: platform
slug: relationalai-authentication
source_filename: relationalai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.relational.ai/build/setup + https://github.com/RelationalAI/rai-agent-skills\nnotes: >-\n  RelationalAI runs as a Native App inside Snowflake. There is no standalone\n  REST/OAuth token surface — authentication is delegated to Snowflake. The\n  PyRel (`relationalai`) SDK and the `rai` CLI connect using a Snowflake\n  connection profile (account, user, and Snowflake auth: key-pair, SSO/SAML,\n  or username-password), and platform access is governed by Snowflake roles.\nsummary:\n  types: [snowflake-connection]\n  delegated_to: snowflake\n  roles: [rai_developer]\nschemes:\n- name: SnowflakeConnection\n  type: platform\n  mechanism: Snowflake connection profile (key-pair / SSO / password)\n  granted_via: Snowflake RBAC roles (e.g. rai_developer)\n  sources:\n  - https://docs.relational.ai/build/setup\n  notes: >-\n    Configured via the SDK/CLI connection profile; the RelationalAI Native App\n    must be installed\
  \ in the Snowflake account and the calling user granted the\n    appropriate RelationalAI role.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/relationalai/refs/heads/main/authentication/relationalai-authentication.yml
summary_line: snowflake-connection · 1 scheme
tags:
- Company
- Decision Intelligence
- Knowledge Graph
- Semantic Layer
- Snowflake
- Graph Analytics
- Machine Learning
- Optimization
- Reasoning
- AI
---
