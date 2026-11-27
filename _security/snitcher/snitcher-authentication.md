---
anonymous_access: false
api_key_in: []
api_specs:
- filename: snitcher-contacts-api-openapi.yml
  format: yaml
  label: Snitcher Contacts API
  slug: snitcher-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snitcher/openapi/snitcher-contacts-api-openapi.yml
- filename: snitcher-custom-field-values-api-openapi.yml
  format: yaml
  label: Snitcher Custom Field Values API
  slug: snitcher-custom-field-values-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snitcher/openapi/snitcher-custom-field-values-api-openapi.yml
- filename: snitcher-custom-fields-api-openapi.yml
  format: yaml
  label: Snitcher Custom Fields API
  slug: snitcher-custom-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snitcher/openapi/snitcher-custom-fields-api-openapi.yml
- filename: snitcher-organisations-api-openapi.yml
  format: yaml
  label: Snitcher Organisations API
  slug: snitcher-organisations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snitcher/openapi/snitcher-organisations-api-openapi.yml
- filename: snitcher-segments-api-openapi.yml
  format: yaml
  label: Snitcher Segments API
  slug: snitcher-segments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snitcher/openapi/snitcher-segments-api-openapi.yml
- filename: snitcher-sessions-api-openapi.yml
  format: yaml
  label: Snitcher Sessions API
  slug: snitcher-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snitcher/openapi/snitcher-sessions-api-openapi.yml
- filename: snitcher-user-api-openapi.yml
  format: yaml
  label: Snitcher User API
  slug: snitcher-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snitcher/openapi/snitcher-user-api-openapi.yml
- filename: snitcher-workspaces-api-openapi.yml
  format: yaml
  label: Snitcher Workspaces API
  slug: snitcher-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snitcher/openapi/snitcher-workspaces-api-openapi.yml
auth_types: []
description: Authentication methods published for Snitcher APIs.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Snitcher Authentication
name_suffix: Authentication
oauth_flows: []
overview: Snitcher declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Snitcher
provider_slug: snitcher
scheme_count: 2
schemes:
- evidence: 'Authentication is done via the API key which will be provided to you separately.

    Requests are authenticated by passing your API key as a bearer token in an `Authorization` header.'
  header: Authorization
  how_to_obtain: API key is provided separately by Snitcher.
  location: header
  name: Bearer token
  type: http-bearer
- evidence: No token or API key is required. Spotter authenticates using the `Origin` header of your request, matched against your authorised domains.
  header: Origin
  how_to_obtain: Configure authorised domains in the Snitcher dashboard.
  location: header
  name: Origin header validation
  type: other
slug: snitcher-authentication
source_filename: snitcher-authentication.yml
source_heading: Authentication Profile
source_url: https://help.snitcher.com/en/collections/3453208-security-compliance
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://help.snitcher.com/en/collections/3453208-security-compliance\nsources:\n- https://help.snitcher.com/en/collections/3453208-security-compliance\n- https://help.snitcher.com/en/collections/19751992-partner-program\n- https://docs.snitcher.com/product/spotter/installation.md\n- https://docs.snitcher.com/powered-by-snitcher/ip2company/quickstart.md\ndescription: Authentication methods published for Snitcher APIs.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Authentication is done via the API key which will be provided to you separately.\n\n    Requests are authenticated by passing your API key as a bearer token in an `Authorization` header.'\n  location: header\n  header: Authorization\n  how_to_obtain: API key is provided separately by Snitcher.\n- type: other\n  name: Origin header validation\n  evidence: No token or API key is required. Spotter authenticates\
  \ using the `Origin` header of your request, matched against your authorised\n    domains.\n  location: header\n  header: Origin\n  how_to_obtain: Configure authorised domains in the Snitcher dashboard.\nnote: Only the authentication schemes explicitly described in the provided pages are included.\ndocs: https://help.snitcher.com/en/collections/3453208-security-compliance\n"
source_yaml_url: https://artifacts.apis.io/snitcher/authentication/snitcher-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Visitor Intelligence
- B2B SaaS
- Lead Generation
- Marketing Automation
---
