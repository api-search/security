---
anonymous_access: false
api_key_in: []
api_specs:
- filename: formester-com-openapi-generated.yml
  format: yaml
  label: Formester API
  slug: formester-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formester-com/openapi/_ae-authored/formester-com-openapi-generated.yml
auth_types: []
description: Formester authenticates to monday.com via OAuth 2.0 authorization flow.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Formester Authentication
name_suffix: Authentication
oauth_flows: []
overview: Formester declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Formester
provider_slug: formester-com
scheme_count: 1
schemes:
- evidence: A popup will appear asking you to authorise Formester on monday.com . Review the permissions and click Authorize .
  flows:
  - authorization_code
  how_to_obtain: User authorizes Formester in a monday.com popup during integration setup.
  name: OAuth 2.0
  type: oauth2
slug: formester-com-authentication
source_filename: formester-com-authentication.yml
source_heading: Authentication Profile
source_url: https://help.formester.com/en/article/mondaycom-integration-setup-guide-12x8gbc/
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://help.formester.com/en/article/mondaycom-integration-setup-guide-12x8gbc/\nsources:\n- https://help.formester.com/en/article/mondaycom-integration-setup-guide-12x8gbc/\ndescription: Formester authenticates to monday.com via OAuth 2.0 authorization flow.\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: A popup will appear asking you to authorise Formester on monday.com . Review the permissions and click Authorize .\n  flows:\n  - authorization_code\n  how_to_obtain: User authorizes Formester in a monday.com popup during integration setup.\ndocs: https://help.formester.com/en/article/mondaycom-integration-setup-guide-12x8gbc/\n"
source_yaml_url: https://artifacts.apis.io/formester-com/authentication/formester-com-authentication.yml
summary_line: 1 scheme
tags:
- Form Builder
- Workflow Automation
- No-Code
- AI-enhanced
- Free
---
