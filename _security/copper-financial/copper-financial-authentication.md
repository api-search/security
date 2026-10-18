---
anonymous_access: false
api_key_in: []
api_specs:
- filename: copper-financial-account-api-openapi.yml
  format: yaml
  label: Copper Financial Account API
  slug: copper-financial-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-financial/refs/heads/main/openapi/copper-financial-account-api-openapi.yml
- filename: copper-financial-activities-api-openapi.yml
  format: yaml
  label: Copper Financial Activities API
  slug: copper-financial-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-financial/refs/heads/main/openapi/copper-financial-activities-api-openapi.yml
- filename: copper-financial-companies-api-openapi.yml
  format: yaml
  label: Copper Financial Companies API
  slug: copper-financial-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-financial/refs/heads/main/openapi/copper-financial-companies-api-openapi.yml
- filename: copper-financial-custom-fields-api-openapi.yml
  format: yaml
  label: Copper Financial Custom Fields API
  slug: copper-financial-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-financial/refs/heads/main/openapi/copper-financial-custom-fields-api-openapi.yml
- filename: copper-financial-field-layouts-api-openapi.yml
  format: yaml
  label: Copper Financial Field Layouts API
  slug: copper-financial-field-layouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-financial/refs/heads/main/openapi/copper-financial-field-layouts-api-openapi.yml
- filename: copper-financial-leads-api-openapi.yml
  format: yaml
  label: Copper Financial Leads API
  slug: copper-financial-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-financial/refs/heads/main/openapi/copper-financial-leads-api-openapi.yml
- filename: copper-financial-opportunities-api-openapi.yml
  format: yaml
  label: Copper Financial Opportunities API
  slug: copper-financial-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-financial/refs/heads/main/openapi/copper-financial-opportunities-api-openapi.yml
- filename: copper-financial-people-api-openapi.yml
  format: yaml
  label: Copper Financial People API
  slug: copper-financial-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-financial/refs/heads/main/openapi/copper-financial-people-api-openapi.yml
- filename: copper-financial-related-items-api-openapi.yml
  format: yaml
  label: Copper Financial Related Items API
  slug: copper-financial-related-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-financial/refs/heads/main/openapi/copper-financial-related-items-api-openapi.yml
- filename: copper-financial-tags-api-openapi.yml
  format: yaml
  label: Copper Financial Tags API
  slug: copper-financial-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-financial/refs/heads/main/openapi/copper-financial-tags-api-openapi.yml
- filename: copper-financial-tasks-api-openapi.yml
  format: yaml
  label: Copper Financial Tasks API
  slug: copper-financial-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copper-financial/refs/heads/main/openapi/copper-financial-tasks-api-openapi.yml
auth_types: []
description: Authentication methods for Copper Developer API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Copper Financial Authentication
name_suffix: Authentication
oauth_flows: []
overview: Copper Financial declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Copper Financial
provider_slug: copper-financial
scheme_count: 2
schemes:
- evidence: The Dev API uses token based authentication. You have to include the token in the header of every request, along with the email address of the user who generated the token.
  how_to_obtain: Generate an API token in the Copper web app under System settings > API Keys by clicking the 'GENERATE API KEY' button.
  location: header
  name: API Key
  type: apiKey
- authorize_url: https://app.copper.com/oauth/authorize
  evidence: 'Copper implements the commonly-used Authorization Code Grant flow:'
  flows:
  - authorizationCode
  how_to_obtain: Register your application with Copper to receive a client_id and client_secret, then follow the Authorization Code Grant flow.
  name: OAuth2.0
  scopes:
  - developer/v1/all
  type: oauth2
slug: copper-financial-authentication
source_filename: copper-financial-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.copper.com/introduction/authentication.html
source_yaml: "generated: '2026-10-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.copper.com/introduction/authentication.html\nsources:\n- https://developer.copper.com/introduction/authentication.html\n- https://developer.copper.com/introduction/oauth/index.html\n- https://developer.copper.com/introduction/oauth/quickstart.html\n- https://developer.copper.com/introduction/oauth/flow.html\ndescription: Authentication methods for Copper Developer API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: The Dev API uses token based authentication. You have to include the token in the header of every request, along with the email address\n    of the user who generated the token.\n  location: header\n  how_to_obtain: Generate an API token in the Copper web app under System settings > API Keys by clicking the 'GENERATE API KEY' button.\n- type: oauth2\n  name: OAuth2.0\n  evidence: 'Copper implements the commonly-used Authorization Code Grant flow:'\n\
  \  flows:\n  - authorizationCode\n  authorize_url: https://app.copper.com/oauth/authorize\n  scopes:\n  - developer/v1/all\n  how_to_obtain: Register your application with Copper to receive a client_id and client_secret, then follow the Authorization Code Grant flow.\ndocs: https://developer.copper.com/introduction/authentication.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/copper-financial/refs/heads/main/authentication/copper-financial-authentication.yml
summary_line: 2 schemes
tags:
- Company
- CRM
- Software-as-a-Service
- Sales
- Marketing
---
