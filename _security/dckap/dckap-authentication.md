---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dckap-openapi-generated.yml
  format: yaml
  label: DCKAP API
  slug: dckap-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dckap/openapi/_ae-authored/dckap-openapi-generated.yml
auth_types: []
description: Authentication schemes published by DCKAP
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Dckap Authentication
name_suffix: Authentication
oauth_flows: []
overview: DCKAP declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: DCKAP
provider_slug: dckap
scheme_count: 1
schemes:
- evidence: OAuth 2.0 is an authorization framework that lets DCKAP Integrator access certain data of another application (like e-commerce or ERP or any system).
  flows:
  - authorization_code
  - authorization_code_pkce
  - resource_owner_password_credentials
  - client_credentials
  name: OAuth 2.0
  type: oauth2
slug: dckap-authentication
source_filename: dckap-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.dckap.com/user-guide/account-management/two-factor-authentication/
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.dckap.com/user-guide/account-management/two-factor-authentication/\nsources:\n- https://docs.dckap.com/user-guide/account-management/two-factor-authentication/\n- https://docs.dckap.com/project-manager/systems/authentication-types/\n- https://docs.dckap.com/project-manager/systems/authentication-types/oauth-2-0/\n- https://docs.dckap.com/project-manager/systems/credentials/\ndescription: Authentication schemes published by DCKAP\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: OAuth 2.0 is an authorization framework that lets DCKAP Integrator access certain data of another application (like e-commerce or\n    ERP or any system).\n  flows:\n  - authorization_code\n  - authorization_code_pkce\n  - resource_owner_password_credentials\n  - client_credentials\ndocs: https://docs.dckap.com/user-guide/account-management/two-factor-authentication/\n"
source_yaml_url: https://artifacts.apis.io/dckap/authentication/dckap-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Integration
- ERP
- E-Commerce
- Data Sync
---
