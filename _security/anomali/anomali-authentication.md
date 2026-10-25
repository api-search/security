---
anonymous_access: false
api_key_in: []
api_specs:
- filename: anomali-openapi-generated.yml
  format: yaml
  label: Anomali API
  slug: anomali-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anomali/refs/heads/main/openapi/_ae-authored/anomali-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Anomali Authentication
name_suffix: Authentication
oauth_flows: []
overview: Anomali declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Anomali
provider_slug: anomali
scheme_count: 3
schemes:
- format: apikey <username>:<api_key>
  header: Authorization
  in: header
  name: apikey
  note: Username is the ThreatStream account email; key from My Account. Credentials in the URL are slated for deprecation.
  type: apiKey
- flow: clientCredentials
  name: oauth2
  note: Limited-availability feature; client ID and secret generated in ThreatStream Account Settings.
  tokenUrl: https://api.threatstream.com/oauth/token
  token_lifetime_seconds: 900
  type: oauth2
- name: mcp-apikey
  note: MCP endpoint answers 401 with WWW-Authenticate ApiKey realm="MCP" (probed 2026-10-20).
  resource: https://api.threatstream.com/mcp
  type: apiKey
slug: anomali-authentication
source_filename: anomali-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Anomali authentication\ngenerated: '2026-10-20'\nmethod: searched\nsource: https://docs.anomali.com/Content/ThreatStream%20API/introduction_api.htm\ndocs: https://docs.anomali.com/Content/ThreatStream%20API/introduction_api.htm\nschemes:\n- name: apikey\n  type: apiKey\n  in: header\n  header: Authorization\n  format: \"apikey <username>:<api_key>\"\n  note: Username is the ThreatStream account email; key from My Account. Credentials in the URL are slated for deprecation.\n- name: oauth2\n  type: oauth2\n  flow: clientCredentials\n  tokenUrl: https://api.threatstream.com/oauth/token\n  token_lifetime_seconds: 900\n  note: Limited-availability feature; client ID and secret generated in ThreatStream Account Settings.\n- name: mcp-apikey\n  type: apiKey\n  resource: https://api.threatstream.com/mcp\n  note: MCP endpoint answers 401 with WWW-Authenticate ApiKey realm=\"MCP\" (probed 2026-10-20).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anomali/refs/heads/main/authentication/anomali-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Enterprise
- Cybersecurity
- Threat Intelligence
- Security
- SIEM
- SOAR
- XDR
- Threat Intelligence Platform
---
