---
anonymous_access: false
api_key_in: []
api_specs:
- filename: komo-do-openapi-generated.yml
  format: yaml
  label: Komodo API
  slug: komo-do-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/komo-do/openapi/_ae-authored/komo-do-openapi-generated.yml
auth_types: []
description: Authentication methods as described on Komodo documentation pages.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Komo Do Authentication
name_suffix: Authentication
oauth_flows: []
overview: Komodo declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Komodo
provider_slug: komo-do
scheme_count: 2
schemes:
- evidence: User sign-on supports username/password and OAuth (GitHub, Google, and generic OIDC) .
  name: Username/Password
  type: http-basic
- evidence: User sign-on supports username/password and OAuth (GitHub, Google, and generic OIDC) .
  name: OAuth
  type: oauth2
slug: komo-do-authentication
source_filename: komo-do-authentication.yml
source_heading: Authentication Profile
source_url: https://komo.do/docs/setup
source_yaml: "generated: '2026-10-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://komo.do/docs/setup\nsources:\n- https://komo.do/docs/setup\n- https://komo.do/docs/intro\n- https://komo.do/docs/setup/mongo\n- https://komo.do/docs/setup/ferretdb\ndescription: Authentication methods as described on Komodo documentation pages.\nschemes:\n- type: http-basic\n  name: Username/Password\n  evidence: User sign-on supports username/password and OAuth (GitHub, Google, and generic OIDC) .\n- type: oauth2\n  name: OAuth\n  evidence: User sign-on supports username/password and OAuth (GitHub, Google, and generic OIDC) .\ndocs: https://komo.do/docs/setup\n"
source_yaml_url: https://artifacts.apis.io/komo-do/authentication/komo-do-authentication.yml
summary_line: 2 schemes
tags:
- Company
- DevOps
- Infrastructure
- Automation
- OpenSource
---
