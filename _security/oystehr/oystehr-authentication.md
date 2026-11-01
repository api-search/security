---
anonymous_access: false
api_key_in: []
api_specs:
- filename: oystehr-openapi-generated.yml
  format: yaml
  label: Oystehr API
  slug: oystehr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oystehr/openapi/_ae-authored/oystehr-openapi-generated.yml
auth_types: []
description: Authentication methods supported by Ottehr as described on the documentation pages.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Oystehr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oystehr declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Oystehr
provider_slug: oystehr
scheme_count: 3
schemes:
- evidence: The patient website uses SMS authentication . Users can enter their phone number and will receive a code that they use to authenticate.
  name: SMS authentication
  type: other
- evidence: The staff website uses email and password authentication . Users sign in with an email and a password.
  name: Email and password authentication
  type: other
- evidence: Oystehr supports SMS authentication, email and password authentication, and Single Sign-On authentication (SSO).
  how_to_obtain: Contact Oystehr at [email protected]
  name: Single Sign-On (SSO)
  type: other
slug: oystehr-authentication
source_filename: oystehr-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.oystehr.com/ottehr/customization/authentication/
source_yaml: "generated: '2026-10-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.oystehr.com/ottehr/customization/authentication/\nsources:\n- https://docs.oystehr.com/ottehr/customization/authentication/\n- https://docs.oystehr.com/ottehr/setup/introduction/\n- https://docs.oystehr.com/ottehr/setup/messaging/\n- https://docs.oystehr.com/ottehr/setup/terminology/\ndescription: Authentication methods supported by Ottehr as described on the documentation pages.\nschemes:\n- type: other\n  name: SMS authentication\n  evidence: The patient website uses SMS authentication . Users can enter their phone number and will receive a code that they use to authenticate.\n- type: other\n  name: Email and password authentication\n  evidence: The staff website uses email and password authentication . Users sign in with an email and a password.\n- type: other\n  name: Single Sign-On (SSO)\n  evidence: Oystehr supports SMS authentication, email and password authentication,\
  \ and Single Sign-On authentication (SSO).\n  how_to_obtain: Contact Oystehr at [email protected]\ndocs: https://docs.oystehr.com/ottehr/customization/authentication/\n"
source_yaml_url: https://artifacts.apis.io/oystehr/authentication/oystehr-authentication.yml
summary_line: 3 schemes
tags:
- Company
- HealthTech
- EHR
- API
- DeveloperFirst
---
