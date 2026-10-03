---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bluetriangletechnologies-content-security-policies-api-openapi.yml
  format: yaml
  label: Bluetriangletechnologies Content Security Policies API
  slug: bluetriangletechnologies-content-security-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluetriangletechnologies/refs/heads/main/openapi/bluetriangletechnologies-content-security-policies-api-openapi.yml
- filename: bluetriangletechnologies-event-markers-api-openapi.yml
  format: yaml
  label: Bluetriangletechnologies Event Markers API
  slug: bluetriangletechnologies-event-markers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluetriangletechnologies/refs/heads/main/openapi/bluetriangletechnologies-event-markers-api-openapi.yml
- filename: bluetriangletechnologies-performance-api-openapi.yml
  format: yaml
  label: Bluetriangletechnologies Performance API
  slug: bluetriangletechnologies-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluetriangletechnologies/refs/heads/main/openapi/bluetriangletechnologies-performance-api-openapi.yml
- filename: bluetriangletechnologies-resource-api-openapi.yml
  format: yaml
  label: Bluetriangletechnologies Resource API
  slug: bluetriangletechnologies-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluetriangletechnologies/refs/heads/main/openapi/bluetriangletechnologies-resource-api-openapi.yml
auth_types: []
description: Authentication for Blue Triangle API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Bluetriangletechnologies Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bluetriangletechnologies declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Bluetriangletechnologies
provider_slug: bluetriangletechnologies
scheme_count: 2
schemes:
- evidence: 'The Blue Triangle API requires each request be sent with two headers:'
  header: X-API-Email
  how_to_obtain: Log into the Blue Triangle Portal, click your Profile, and view Profile to find your email address.
  location: header
  name: X-API-Email
  type: apiKey
- evidence: 'The Blue Triangle API requires each request be sent with two headers:'
  header: X-API-Key
  how_to_obtain: Log into the Blue Triangle Portal, click your Profile, and view Profile to find your API key.
  location: header
  name: X-API-Key
  type: apiKey
slug: bluetriangletechnologies-authentication
source_filename: bluetriangletechnologies-authentication.yml
source_heading: Authentication Profile
source_url: https://help.bluetriangle.com/help-center/why-is-the-api-responding-with-403-incorrect-email-or-api-key-provided-how-do-i-find-my-api-key-email.md
source_yaml: "generated: '2026-09-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://help.bluetriangle.com/help-center/why-is-the-api-responding-with-403-incorrect-email-or-api-key-provided-how-do-i-find-my-api-key-email.md\nsources:\n- https://help.bluetriangle.com/help-center/why-is-the-api-responding-with-403-incorrect-email-or-api-key-provided-how-do-i-find-my-api-key-email.md\n- https://help.bluetriangle.com/help-center/getting-started.md\n- https://help.bluetriangle.com/help-center/getting-started-with-the-bt-portal.md\n- https://help.bluetriangle.com/help-center/quick-start-guide-for-instrumenting-android-mobile-applications.md\ndescription: Authentication for Blue Triangle API\nschemes:\n- type: apiKey\n  name: X-API-Email\n  evidence: 'The Blue Triangle API requires each request be sent with two headers:'\n  location: header\n  header: X-API-Email\n  how_to_obtain: Log into the Blue Triangle Portal, click your Profile, and view Profile to find your\
  \ email address.\n- type: apiKey\n  name: X-API-Key\n  evidence: 'The Blue Triangle API requires each request be sent with two headers:'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Log into the Blue Triangle Portal, click your Profile, and view Profile to find your API key.\ndocs: https://help.bluetriangle.com/help-center/why-is-the-api-responding-with-403-incorrect-email-or-api-key-provided-how-do-i-find-my-api-key-email.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluetriangletechnologies/refs/heads/main/authentication/bluetriangletechnologies-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Analytics
- Revenue Assurance
- Digital Experience
- Artificial Intelligence
---
