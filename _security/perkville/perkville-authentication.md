---
anonymous_access: false
api_key_in: []
api_specs:
- filename: perkville-openapi-generated.yml
  format: yaml
  label: Perkville API
  slug: perkville-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/perkville/openapi/_ae-authored/perkville-openapi-generated.yml
auth_types: []
description: Authentication methods described on the Perkville authentication page.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Perkville Authentication
name_suffix: Authentication
oauth_flows: []
overview: Perkville declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Perkville
provider_slug: perkville
scheme_count: 1
schemes:
- evidence: 'Resource Owner (Password) Grant: A token only becomes invalid if your API client is deactivated (reserved for cases of abuse), or if the admin user associated with the token loses staff status at a business.'
  flows:
  - password
  name: Resource Owner (Password) Grant
  type: oauth2
slug: perkville-authentication
source_filename: perkville-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.perkville.com/integrations/integrating-perkville/integrating-your-app-with-perkville/authentication.md
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.perkville.com/integrations/integrating-perkville/integrating-your-app-with-perkville/authentication.md\nsources:\n- https://docs.perkville.com/integrations/integrating-perkville/integrating-your-app-with-perkville/authentication.md\n- https://docs.perkville.com/guides/signing-up-with-perkville.md\n- https://docs.perkville.com/features/settings/location-setup.md\n- https://docs.perkville.com/features/settings/location-setup/locations.md\ndescription: Authentication methods described on the Perkville authentication page.\nschemes:\n- type: oauth2\n  name: Resource Owner (Password) Grant\n  evidence: 'Resource Owner (Password) Grant: A token only becomes invalid if your API client is deactivated (reserved for cases of abuse), or\n    if the admin user associated with the token loses staff status at a business.'\n  flows:\n  - password\ndocs: https://docs.perkville.com/integrations/integrating-perkville/integrating-your-app-with-perkville/authentication.md\n\
  note: 2 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/perkville/authentication/perkville-authentication.yml
summary_line: 1 scheme
tags:
- Loyalty
- Software-as-a-Service
- Customer Engagement
- Referral Program
- Marketing
---
