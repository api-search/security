---
anonymous_access: false
api_key_in: []
api_specs:
- filename: frazzlecrm-com-openapi-generated.yml
  format: yaml
  label: FrazzleCRM API
  slug: frazzlecrm-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/frazzlecrm-com/openapi/_ae-authored/frazzlecrm-com-openapi-generated.yml
auth_types: []
description: FrazzleCRM uses an API key that is sent as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: FrazzleCRM Authentication
name_suffix: Authentication
oauth_flows: []
overview: FrazzleCRM declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: FrazzleCRM
provider_slug: frazzlecrm-com
scheme_count: 1
schemes:
- evidence: 'Authorization: Bearer frz_your_key'
  header: Authorization
  how_to_obtain: Create a key in Settings → API Keys; the key starts with frz_
  location: header
  name: API Key
  type: http-bearer
slug: frazzlecrm-com-authentication
source_filename: frazzlecrm-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.frazzlecrm.com/ai
source_yaml: "generated: '2026-11-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.frazzlecrm.com/ai\nsources:\n- https://www.frazzlecrm.com/ai\n- https://www.frazzlecrm.com/templates/saas-trial-onboarding\n- https://www.frazzlecrm.com/templates/course-student-onboarding\n- https://www.frazzlecrm.com/templates/agency-client-onboarding\ndescription: FrazzleCRM uses an API key that is sent as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Authorization: Bearer frz_your_key'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in Settings → API Keys; the key starts with frz_\ndocs: https://www.frazzlecrm.com/ai\n"
source_yaml_url: https://artifacts.apis.io/frazzlecrm-com/authentication/frazzlecrm-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- CRM
- Automation
- Artificial Intelligence
- Software-as-a-Service
---
