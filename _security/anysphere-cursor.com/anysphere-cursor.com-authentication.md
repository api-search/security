---
anonymous_access: false
api_key_in: []
api_specs:
- filename: anysphere-cursor.com-originservice-api-openapi.yml
  format: yaml
  label: Anysphere Cursor.com Origin Service API
  slug: anysphere-cursor.com-originservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anysphere-cursor.com/refs/heads/main/openapi/anysphere-cursor.com-originservice-api-openapi.yml
auth_types: []
description: 'Service accounts authenticate using their API key. Use the key in the Authorization header when making requests to the Cloud Agents API :'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Anysphere Cursor.Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Anysphere Cursor.com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Anysphere Cursor.com
provider_slug: anysphere-cursor.com
scheme_count: 1
schemes:
- evidence: 'Service accounts authenticate using their API key. Use the key in the Authorization header when making requests to the Cloud Agents API :'
  header: Authorization
  how_to_obtain: Create a service account in the Cursor Dashboard → Settings → API Keys → Service Accounts, then copy the generated API key.
  location: header
  name: Service Account API Key
  type: http-bearer
slug: anysphere-cursor.com-authentication
source_filename: anysphere-cursor.com-authentication.yml
source_heading: Authentication Profile
source_url: https://cursor.com/docs/account/enterprise/service-accounts
source_yaml: "generated: '2026-09-25'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://cursor.com/docs/account/enterprise/service-accounts\nsources:\n- https://cursor.com/docs/account/enterprise/service-accounts\n- https://cursor.com/docs/get-started/quickstart\n- https://cursor.com/docs/cloud-agent/setup\ndescription: 'Service accounts authenticate using their API key. Use the key in the Authorization header when making requests to the Cloud Agents\n  API :'\nschemes:\n- type: http-bearer\n  name: Service Account API Key\n  evidence: 'Service accounts authenticate using their API key. Use the key in the Authorization header when making requests to the Cloud Agents\n    API :'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a service account in the Cursor Dashboard → Settings → API Keys → Service Accounts, then copy the generated API key.\ndocs: https://cursor.com/docs/account/enterprise/service-accounts\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anysphere-cursor.com/refs/heads/main/authentication/anysphere-cursor.com-authentication.yml
summary_line: 1 scheme
tags:
- AI Coding
- Development Tools
- Cloud Agents
- CLI
- Enterprise Software
---
