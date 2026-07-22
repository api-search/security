---
api_key_in: []
auth_types:
- none
- session
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Mindsdb Authentication
name_suffix: Authentication
oauth_flows: []
overview: MindsDB secures its APIs with none, session, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MindsDB
provider_slug: mindsdb
scheme_count: 3
schemes:
- description: Default local server (http://127.0.0.1:47334) requires no authentication.
  name: self-hosted-no-auth
  sources:
  - https://github.com/mindsdb/mindsdb_python_sdk
  type: none
- description: MindsDB Cloud authenticates with login (email) + password; the SDK/HTTP client then carries a session cookie. Managed/Pro instances use the same login flow with is_managed set.
  login_host: https://cloud.mindsdb.com
  name: cloud-session
  sources:
  - https://github.com/mindsdb/mindsdb_python_sdk
  - https://github.com/mindsdb/mindsdb-js-sdk
  type: session
- description: The built-in MCP server (FastMCP) supports optional OAuth (mindsdb/api/mcp/oauth.py).
  name: mcp-oauth
  optional: true
  sources:
  - https://github.com/mindsdb/engine
  type: oauth2
slug: mindsdb-authentication
source_filename: mindsdb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.mindsdb.com/rest/authentication + mindsdb_python_sdk / mindsdb-js-sdk READMEs\nsummary:\n  types: [none, session, oauth2]\n  notes: >-\n    MindsDB is primarily self-hosted software. Against a local MindsDB server no\n    authentication is required. Against MindsDB Cloud the SDKs authenticate with\n    a login (email) + password, which establishes a session cookie used by the\n    HTTP REST API. The built-in MCP server can optionally require OAuth.\nschemes:\n  - name: self-hosted-no-auth\n    type: none\n    description: Default local server (http://127.0.0.1:47334) requires no authentication.\n    sources: [https://github.com/mindsdb/mindsdb_python_sdk]\n  - name: cloud-session\n    type: session\n    description: >-\n      MindsDB Cloud authenticates with login (email) + password; the SDK/HTTP\n      client then carries a session cookie. Managed/Pro instances use the same\n      login flow with is_managed set.\n\
  \    login_host: https://cloud.mindsdb.com\n    sources:\n      - https://github.com/mindsdb/mindsdb_python_sdk\n      - https://github.com/mindsdb/mindsdb-js-sdk\n  - name: mcp-oauth\n    type: oauth2\n    description: The built-in MCP server (FastMCP) supports optional OAuth (mindsdb/api/mcp/oauth.py).\n    optional: true\n    sources: [https://github.com/mindsdb/engine]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mindsdb/refs/heads/main/authentication/mindsdb-authentication.yml
summary_line: none/session/oauth2 · 3 schemes
tags:
- Company
- Artificial Intelligence
- Machine Learning
- AI Agents
- Data
- Database
- SQL
- Knowledge Base
- MCP
- Open Source
---
