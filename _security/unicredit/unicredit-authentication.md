---
anonymous_access: false
api_key_in: []
api_specs:
- filename: unicredit-openapi-generated.yml
  format: yaml
  label: UniCredit API
  slug: unicredit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unicredit/refs/heads/main/openapi/_ae-authored/unicredit-openapi-generated.yml
auth_types: []
description: Authentication schemes for UniCredit APIs as described on the Getting Started page.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Unicredit Authentication
name_suffix: Authentication
oauth_flows: []
overview: UniCredit declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: UniCredit
provider_slug: unicredit
scheme_count: 1
schemes:
- evidence: A TPP can interact with UniCredit APIs by presenting a valid QWAC (Qualified Web Authentication Certificate) certificate, according to the eIDAS Regulation.
  name: QWAC certificate
  type: mtls
slug: unicredit-authentication
source_filename: unicredit-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.unicredit.eu/support/getting-started-public
source_yaml: "generated: '2026-10-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.unicredit.eu/support/getting-started-public\nsources:\n- https://developer.unicredit.eu/support/getting-started-public\ndescription: Authentication schemes for UniCredit APIs as described on the Getting Started page.\nschemes:\n- type: mtls\n  name: QWAC certificate\n  evidence: A TPP can interact with UniCredit APIs by presenting a valid QWAC (Qualified Web Authentication Certificate) certificate, according\n    to the eIDAS Regulation.\ndocs: https://developer.unicredit.eu/support/getting-started-public\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unicredit/refs/heads/main/authentication/unicredit-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Banking
- Financial Services
- Europe
- Corporate Banking
---
