---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Digital.ai Agility as described in the documentation.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Numerify Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Numerify declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Numerify
provider_slug: numerify-com
scheme_count: 3
schemes:
- evidence: Digital.ai Agility stores each member's username and password.
  name: Username/Password
  type: other
- evidence: Digital.ai Agility stores the username and delegates authentication of the username and password to active directory.
  name: Windows Integrated Authentication
  type: other
- evidence: Digital.ai Agility is configured to receive the username in an HTTP header, which is passed to the application by the SSO infrastructure.
  location: header
  name: Single Sign On Authentication (On-Premise)
  type: other
slug: numerify-com-authentication
source_filename: numerify-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.digital.ai/agility/docs/tags/application-authentication
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.digital.ai/agility/docs/tags/application-authentication\nsources:\n- https://docs.digital.ai/agility/docs/tags/application-authentication\n- https://docs.digital.ai/agility/docs/tags/federated-authentication\n- https://docs.digital.ai/agility/docs/agility/authentication\n- https://docs.digital.ai/agility/docs/agility/configuring-saml-sso-using-federated-authentication\ndescription: Authentication methods for Digital.ai Agility as described in the documentation.\nschemes:\n- type: other\n  name: Username/Password\n  evidence: Digital.ai Agility stores each member's username and password.\n- type: other\n  name: Windows Integrated Authentication\n  evidence: Digital.ai Agility stores the username and delegates authentication of the username and password to active directory.\n- type: other\n  name: Single Sign On Authentication (On-Premise)\n  evidence: Digital.ai Agility\
  \ is configured to receive the username in an HTTP header, which is passed to the application by the SSO infrastructure.\n  location: header\ndocs: https://docs.digital.ai/agility/docs/tags/application-authentication\n"
source_yaml_url: https://artifacts.apis.io/numerify-com/authentication/numerify-com-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Venture
- Startup
- Acquired
- API
---
