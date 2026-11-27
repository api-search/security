---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: createavataaars Authentication
name_suffix: Authentication
oauth_flows: []
overview: createavataaars declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: createavataaars
provider_slug: createavataaars-com
scheme_count: 2
schemes:
- applies_to: MCP tools list_styles, list_templates, list_attributes, random_avatar, create_avatar, avatar_for_name, share_link, render_avatar
  evidence: Nothing to install and no key. It is a URL.
  name: none
  type: none
- applies_to: MCP account tools save_avatar, list_my_avatars, set_account_avatar
  evidence: The account tools ask you to sign in the first time.
  name: kurcz-account-sign-in
  type: interactive-sign-in
slug: createavataaars-com-authentication
source_filename: createavataaars-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://createavataaars.com/mcp\ndocs: https://createavataaars.com/mcp\nnote: There is no REST API and no OpenAPI (https://createavataaars.com/api says \"There is no API yet\"). The remote MCP server\n  needs no key; account tools prompt the user to sign in to a Kurcz account. The sign-in mechanism is not documented.\nschemes:\n- name: none\n  type: none\n  applies_to: MCP tools list_styles, list_templates, list_attributes, random_avatar, create_avatar, avatar_for_name, share_link, render_avatar\n  evidence: Nothing to install and no key. It is a URL.\n- name: kurcz-account-sign-in\n  type: interactive-sign-in\n  applies_to: MCP account tools save_avatar, list_my_avatars, set_account_avatar\n  evidence: The account tools ask you to sign in the first time.\n"
source_yaml_url: https://artifacts.apis.io/createavataaars-com/authentication/createavataaars-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Avatars
- Avatar Generator
- Profile Pictures
- Illustration
- MCP
- AI Agents
---
