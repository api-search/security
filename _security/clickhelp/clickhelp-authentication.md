---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for ClickHelp as documented.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Clickhelp Authentication
name_suffix: Authentication
oauth_flows: []
overview: ClickHelp declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ClickHelp
provider_slug: clickhelp
scheme_count: 2
schemes:
- evidence: This is the default authentication option, and it doesn't require any additional setup.
  how_to_obtain: Credentials are emailed to the user when the account is created and can be changed via the User Profile.
  name: Native ClickHelp credentials
  type: http-basic
- evidence: ClickHelp supports the OpenID Connect technology of single sign-on.
  how_to_obtain: Configured through the Single Sign-On (SSO) settings; uses the identity provider's OpenID Connect flow.
  name: SSO
  type: oauth2
slug: clickhelp-authentication
source_filename: clickhelp-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.clickhelp.com/articles/clickhelp-user-manual/authentication.md
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.clickhelp.com/articles/clickhelp-user-manual/authentication.md\nsources:\n- https://docs.clickhelp.com/articles/clickhelp-user-manual/authentication.md\n- https://docs.clickhelp.com/articles/clickhelp-user-manual/two-factor-authentication-2fa.md\n- https://docs.clickhelp.com/articles/clickhelp-user-manual/authentication-across-documentation-sites.md\n- https://docs.clickhelp.com/articles/clickhelp-user-manual/get-api-key.md\ndescription: Authentication methods for ClickHelp as documented.\nschemes:\n- type: http-basic\n  name: Native ClickHelp credentials\n  evidence: This is the default authentication option, and it doesn't require any additional setup.\n  how_to_obtain: Credentials are emailed to the user when the account is created and can be changed via the User Profile.\n- type: oauth2\n  name: SSO\n  evidence: ClickHelp supports the OpenID Connect technology of\
  \ single sign-on.\n  how_to_obtain: Configured through the Single Sign-On (SSO) settings; uses the identity provider's OpenID Connect flow.\ndocs: https://docs.clickhelp.com/articles/clickhelp-user-manual/authentication.md\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/clickhelp/authentication/clickhelp-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Documentation
- AI
- SaaS
- Technical Writing
---
