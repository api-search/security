---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes published on the referenced OneDev documentation pages.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Onedev Authentication
name_suffix: Authentication
oauth_flows: []
overview: OneDev declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: OneDev
provider_slug: onedev
scheme_count: 1
schemes:
- evidence: 'Upon clicking this icon, office 365 login screen will be shown:'
  flows:
  - authorization_code
  how_to_obtain: Generate a refresh token via the icon on the mail setting page, which opens the Office 365 login screen for the user to sign in and accept permissions.
  name: Office 365
  type: oauth2
slug: onedev-authentication
source_filename: onedev-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.onedev.io/tutorials/security/oauth-with-office365
source_yaml: "generated: '2026-10-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.onedev.io/tutorials/security/oauth-with-office365\nsources:\n- https://docs.onedev.io/tutorials/security/oauth-with-office365\n- https://docs.onedev.io/tutorials/security/auth-source-switch\n- https://docs.onedev.io/tutorials/security/manage-access-tokens\n- https://docs.onedev.io/administration-guide/https-setup\ndescription: Authentication schemes published on the referenced OneDev documentation pages.\nschemes:\n- type: oauth2\n  name: Office 365\n  evidence: 'Upon clicking this icon, office 365 login screen will be shown:'\n  flows:\n  - authorization_code\n  how_to_obtain: Generate a refresh token via the icon on the mail setting page, which opens the Office 365 login screen for the user to sign\n    in and accept permissions.\ndocs: https://docs.onedev.io/tutorials/security/oauth-with-office365\n"
source_yaml_url: https://artifacts.apis.io/onedev/authentication/onedev-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Development
- CI/CD
- Git
- Automation
---
