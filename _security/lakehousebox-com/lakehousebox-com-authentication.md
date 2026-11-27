---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lakehousebox-com-openapi-generated.yml
  format: yaml
  label: LakehouseBox API
  slug: lakehousebox-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lakehousebox-com/openapi/_ae-authored/lakehousebox-com-openapi-generated.yml
auth_types: []
description: Authentication for LakehouseBox is performed via a bearer token obtained through the CLI login flow.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: LakehouseBox Authentication
name_suffix: Authentication
oauth_flows: []
overview: LakehouseBox declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: LakehouseBox
provider_slug: lakehousebox-com
scheme_count: 1
schemes:
- evidence: 'The CLI receives a key that acts as you : it can do what you can do on the website, in every organisation you belong to, for 30 days'
  header: Authorization
  how_to_obtain: Run `lhbox login`, which opens a browser where the user clicks Allow; the CLI then saves the key to ~/.config/lhbox/credentials.json and uses it for subsequent requests.
  location: header
  name: LHBOX_API_KEY
  type: http-bearer
slug: lakehousebox-com-authentication
source_filename: lakehousebox-com-authentication.yml
source_heading: Authentication Profile
source_url: https://lakehousebox.com/docs/access/credentials/
source_yaml: "generated: '2026-11-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://lakehousebox.com/docs/access/credentials/\nsources:\n- https://lakehousebox.com/docs/access/credentials/\n- https://lakehousebox.com/docs/access/credentials\n- https://lakehousebox.com/docs/quickstart/\n- https://lakehousebox.com/docs/agent-setup/\ndescription: Authentication for LakehouseBox is performed via a bearer token obtained through the CLI login flow.\nschemes:\n- type: http-bearer\n  name: LHBOX_API_KEY\n  evidence: 'The CLI receives a key that acts as you : it can do what you can do on the website, in every organisation you belong to, for 30 days'\n  location: header\n  header: Authorization\n  how_to_obtain: Run `lhbox login`, which opens a browser where the user clicks Allow; the CLI then saves the key to ~/.config/lhbox/credentials.json\n    and uses it for subsequent requests.\ndocs: https://lakehousebox.com/docs/access/credentials/\n"
source_yaml_url: https://artifacts.apis.io/lakehousebox-com/authentication/lakehousebox-com-authentication.yml
summary_line: 1 scheme
tags:
- Data Infrastructure
- AI Agents
- Cloud Services
- Open Data
- Lakehouse
---
