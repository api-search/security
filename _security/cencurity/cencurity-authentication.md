---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes described in Cencurity documentation
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Cencurity Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cencurity declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Cencurity
provider_slug: cencurity
scheme_count: 2
schemes:
- evidence: Enter your API key.
  how_to_obtain: User enters the API key in the VS Code extension settings.
  name: Provider API Key
  type: apiKey
- evidence: Enter the issued API key on the login screen.
  how_to_obtain: Copy the CENCURITY_BOOTSTRAP_TENANT_API_KEY value from the bootstrap_tenant_customer_api_key.txt file generated after starting the Docker containers.
  name: Bootstrap Tenant API Key
  type: apiKey
slug: cencurity-authentication
source_filename: cencurity-authentication.yml
source_heading: Authentication Profile
source_url: https://cencurity.com/docs/getting-started/quickstart
source_yaml: "generated: '2026-10-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://cencurity.com/docs/getting-started/quickstart\nsources:\n- https://cencurity.com/docs/getting-started/quickstart\n- https://cencurity.com/docs/getting-started/run-with-docker\n- https://cencurity.com/docs/getting-started/connect-through-proxy\ndescription: Authentication schemes described in Cencurity documentation\nschemes:\n- type: apiKey\n  name: Provider API Key\n  evidence: Enter your API key.\n  how_to_obtain: User enters the API key in the VS Code extension settings.\n- type: apiKey\n  name: Bootstrap Tenant API Key\n  evidence: Enter the issued API key on the login screen.\n  how_to_obtain: Copy the CENCURITY_BOOTSTRAP_TENANT_API_KEY value from the bootstrap_tenant_customer_api_key.txt file generated after starting\n    the Docker containers.\ndocs: https://cencurity.com/docs/getting-started/quickstart\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cencurity/refs/heads/main/authentication/cencurity-authentication.yml
summary_line: 2 schemes
tags:
- AI Security
- LLM Proxy
- Real-time Threat Monitoring
- Audit Reporting
- Developer Tools
- Policy Enforcement
---
