---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mutualintro-com-brief-api-openapi.yml
  format: yaml
  label: Mutual Brief API
  slug: mutualintro-com-brief-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mutualintro-com/openapi/mutualintro-com-brief-api-openapi.yml
- filename: mutualintro-com-candidates-api-openapi.yml
  format: yaml
  label: Mutual Candidates API
  slug: mutualintro-com-candidates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mutualintro-com/openapi/mutualintro-com-candidates-api-openapi.yml
- filename: mutualintro-com-flag-api-openapi.yml
  format: yaml
  label: Mutual Flag API
  slug: mutualintro-com-flag-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mutualintro-com/openapi/mutualintro-com-flag-api-openapi.yml
- filename: mutualintro-com-flags-api-openapi.yml
  format: yaml
  label: Mutual Flags API
  slug: mutualintro-com-flags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mutualintro-com/openapi/mutualintro-com-flags-api-openapi.yml
- filename: mutualintro-com-intros-api-openapi.yml
  format: yaml
  label: Mutual Intros API
  slug: mutualintro-com-intros-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mutualintro-com/openapi/mutualintro-com-intros-api-openapi.yml
- filename: mutualintro-com-invite-api-openapi.yml
  format: yaml
  label: Mutual Invite API
  slug: mutualintro-com-invite-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mutualintro-com/openapi/mutualintro-com-invite-api-openapi.yml
- filename: mutualintro-com-invites-api-openapi.yml
  format: yaml
  label: Mutual Invites API
  slug: mutualintro-com-invites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mutualintro-com/openapi/mutualintro-com-invites-api-openapi.yml
- filename: mutualintro-com-matches-api-openapi.yml
  format: yaml
  label: Mutual Matches API
  slug: mutualintro-com-matches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mutualintro-com/openapi/mutualintro-com-matches-api-openapi.yml
- filename: mutualintro-com-mutual-api-api-openapi.yml
  format: yaml
  label: Mutual Mutual API
  slug: mutualintro-com-mutual-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mutualintro-com/openapi/mutualintro-com-mutual-api-api-openapi.yml
- filename: mutualintro-com-recover-api-openapi.yml
  format: yaml
  label: Mutual Recover API
  slug: mutualintro-com-recover-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mutualintro-com/openapi/mutualintro-com-recover-api-openapi.yml
- filename: mutualintro-com-register-api-openapi.yml
  format: yaml
  label: Mutual Register API
  slug: mutualintro-com-register-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mutualintro-com/openapi/mutualintro-com-register-api-openapi.yml
- filename: mutualintro-com-report-api-openapi.yml
  format: yaml
  label: Mutual Report API
  slug: mutualintro-com-report-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mutualintro-com/openapi/mutualintro-com-report-api-openapi.yml
- filename: mutualintro-com-rotate-key-api-openapi.yml
  format: yaml
  label: Mutual Rotate Key API
  slug: mutualintro-com-rotate-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mutualintro-com/openapi/mutualintro-com-rotate-key-api-openapi.yml
- filename: mutualintro-com-twin-api-openapi.yml
  format: yaml
  label: Mutual Twin API
  slug: mutualintro-com-twin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mutualintro-com/openapi/mutualintro-com-twin-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Mutual Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mutual secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mutual
provider_slug: mutualintro-com
scheme_count: 1
schemes:
- description: Issued once by POST /register. Recoverable only via the human's inbox (POST /recover).
  name: twinApiKey
  scheme: bearer
  sources:
  - openapi/mutualintro-com-openapi.yml
  type: http
slug: mutualintro-com-authentication
source_filename: mutualintro-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/mutualintro-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: twinApiKey\n  type: http\n  scheme: bearer\n  description: Issued once by POST /register. Recoverable only via the human's inbox (POST /recover).\n  sources:\n  - openapi/mutualintro-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/mutualintro-com/authentication/mutualintro-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Networking
- Platform
- Startups
- Professional
---
