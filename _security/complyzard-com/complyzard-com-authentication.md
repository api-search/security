---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Complyzard Authentication
name_suffix: Authentication
oauth_flows: []
overview: Complyzard declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Complyzard
provider_slug: complyzard-com
scheme_count: 2
schemes:
- description: Public search does not require a Complyzard account.
  scope: MCP document search
  type: none
- description: Sign in to download using your membership or a download credit.
  scope: downloads
  type: account-session
slug: complyzard-com-authentication
source_filename: complyzard-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://complyzard.com/integrations\ndocs: https://complyzard.com/integrations\nschemes:\n- type: none\n  scope: MCP document search\n  description: \"Public search does not require a Complyzard account.\"\n- type: account-session\n  scope: downloads\n  description: \"Sign in to download using your membership or a download credit.\"\nnote: No OAuth protected-resource metadata was found on complyzard.com (pre-flight well-known probe). The docs do not describe how an MCP client authenticates for downloads; sign-in is documented only for the website.\n"
source_yaml_url: https://artifacts.apis.io/complyzard-com/authentication/complyzard-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Compliance
- Governance Risk and Compliance
- Information Security
- Privacy
- AI Governance
- Document Marketplace
- MCP
---
