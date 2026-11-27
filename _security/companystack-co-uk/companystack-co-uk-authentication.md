---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: CompanyStack Authentication
name_suffix: Authentication
oauth_flows: []
overview: CompanyStack declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: CompanyStack
provider_slug: companystack-co-uk
scheme_count: 2
schemes:
- applies_to: https://api.companystack.co.uk/mcp
  evidence: 'Optional: your CompanyStack API key (starts with cs_). Leave it out to sign in with CompanyStack (OAuth) instead. Create an account free at https://companystack.co.uk/signup?product=api'
  in: header
  key_prefix: cs_
  name: X-Api-Key
  required: false
  type: apiKey
- applies_to: https://api.companystack.co.uk/mcp
  evidence: Leave it out to sign in with CompanyStack (OAuth) instead.
  name: CompanyStack sign-in
  note: Flows, endpoints and scopes are not published in the registry entry; v0.1.0 described the 401 challenge as the signal that sign-in is offered.
  type: oauth2
slug: companystack-co-uk-authentication
source_filename: companystack-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://registry.modelcontextprotocol.io/v0/servers?search=companystack\ndocs: https://companystack.co.uk/developers/mcp\nnote: companystack.co.uk refused TCP connections on 2026-11-04 (ECONNREFUSED), so the docs page could not be read; the scheme below is quoted from the provider's own official MCP Registry entry uk.co.companystack/mcp v0.1.1 (isLatest).\nschemes:\n- name: X-Api-Key\n  type: apiKey\n  in: header\n  key_prefix: cs_\n  applies_to: https://api.companystack.co.uk/mcp\n  required: false\n  evidence: \"Optional: your CompanyStack API key (starts with cs_). Leave it out to sign in with CompanyStack (OAuth) instead. Create an account free at https://companystack.co.uk/signup?product=api\"\n- name: CompanyStack sign-in\n  type: oauth2\n  applies_to: https://api.companystack.co.uk/mcp\n  evidence: \"Leave it out to sign in with CompanyStack (OAuth) instead.\"\n  note: Flows, endpoints and scopes are not published in\
  \ the registry entry; v0.1.0 described the 401 challenge as the signal that sign-in is offered.\n"
source_yaml_url: https://artifacts.apis.io/companystack-co-uk/authentication/companystack-co-uk-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Company Data
- Companies House
- United Kingdom
- KYB
- Business Verification
- MCP
---
