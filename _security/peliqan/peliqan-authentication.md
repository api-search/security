---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Peliqan as documented
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Peliqan Authentication
name_suffix: Authentication
oauth_flows: []
overview: Peliqan declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Peliqan
provider_slug: peliqan
scheme_count: 1
schemes:
- authorize_url: <https://app.eu.peliqan.io/oauth2/authorize>
  evidence: Click "Connect AdminPulse" to connect your AdminPulse account to Peliqan with OAuth.
  flows:
  - authorization_code
  how_to_obtain: Obtain credentials by completing the OAuth authorization flow via the Peliqan authorization endpoint.
  name: Peliqan
  scopes:
  - openid
  - email
  - profile
  type: oauth2
slug: peliqan-authentication
source_filename: peliqan-authentication.yml
source_heading: Authentication Profile
source_url: https://help.peliqan.io/custom-mcp-with-o-auth.md
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://help.peliqan.io/custom-mcp-with-o-auth.md\nsources:\n- https://help.peliqan.io/custom-mcp-with-o-auth.md\n- https://help.peliqan.io/adminpulse-getting-started-in-peliqan.md\n- https://help.peliqan.io/adsolut-getting-started-in-peliqan.md\n- https://help.peliqan.io/afas-getting-started-in-peliqan.md\ndescription: Authentication methods for Peliqan as documented\nschemes:\n- type: oauth2\n  name: Peliqan\n  evidence: Click \"Connect AdminPulse\" to connect your AdminPulse account to Peliqan with OAuth.\n  flows:\n  - authorization_code\n  authorize_url: <https://app.eu.peliqan.io/oauth2/authorize>\n  scopes:\n  - openid\n  - email\n  - profile\n  how_to_obtain: Obtain credentials by completing the OAuth authorization flow via the Peliqan authorization endpoint.\ndocs: https://help.peliqan.io/custom-mcp-with-o-auth.md\n"
source_yaml_url: https://artifacts.apis.io/peliqan/authentication/peliqan-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Data Platform
- AI
- ETL
- Reverse ETL
---
