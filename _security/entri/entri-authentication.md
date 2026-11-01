---
anonymous_access: false
api_key_in: []
api_specs:
- filename: entri-openapi-generated.yml
  format: yaml
  label: Entri API
  slug: entri-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/entri/openapi/_ae-authored/entri-openapi-generated.yml
auth_types: []
description: Authentication methods for Entri DNS Provider onboarding
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Entri Authentication
name_suffix: Authentication
oauth_flows: []
overview: Entri declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Entri
provider_slug: entri
scheme_count: 3
schemes:
- evidence: 'Choose one of the three authentication methods:'
  how_to_obtain: Provide Client ID, Client secret, Authorization URL, and Token URL in the OAuth credentials fields.
  name: OAuth 2.0
  type: oauth2
- evidence: 'Choose one of the three authentication methods:'
  header: Authorization
  how_to_obtain: Enter the static API key as an Authentication Parameter with the header name `Authorization`.
  location: header
  name: Basic Auth
  type: http-bearer
- evidence: 'Choose one of the three authentication methods:'
  how_to_obtain: Entri will collect the username and password directly from the user during the login flow.
  name: Login (with optional MFA)
  type: http-basic
slug: entri-authentication
source_filename: entri-authentication.yml
source_heading: Authentication Profile
source_url: https://help.entri.com/articles/1668259832-supported-multi-factor-authentication-mfa-methods
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://help.entri.com/articles/1668259832-supported-multi-factor-authentication-mfa-methods\nsources:\n- https://help.entri.com/articles/1668259832-supported-multi-factor-authentication-mfa-methods\n- https://developers.entri.com/getting-started.md\n- https://developers.entri.com/network/dns-provider-onboarding.md\ndescription: Authentication methods for Entri DNS Provider onboarding\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: 'Choose one of the three authentication methods:'\n  how_to_obtain: Provide Client ID, Client secret, Authorization URL, and Token URL in the OAuth credentials fields.\n- type: http-bearer\n  name: Basic Auth\n  evidence: 'Choose one of the three authentication methods:'\n  location: header\n  header: Authorization\n  how_to_obtain: Enter the static API key as an Authentication Parameter with the header name `Authorization`.\n- type: http-basic\n\
  \  name: Login (with optional MFA)\n  evidence: 'Choose one of the three authentication methods:'\n  how_to_obtain: Entri will collect the username and password directly from the user during the login flow.\ndocs: https://help.entri.com/articles/1668259832-supported-multi-factor-authentication-mfa-methods\n"
source_yaml_url: https://artifacts.apis.io/entri/authentication/entri-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Domain
- Integration
- Software-as-a-Service
---
