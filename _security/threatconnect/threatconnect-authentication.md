---
anonymous_access: false
api_key_in: []
api_specs:
- filename: threatconnect-apps-api-openapi.yml
  format: yaml
  label: ThreatConnect Apps API
  slug: threatconnect-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatconnect/refs/heads/main/openapi/threatconnect-apps-api-openapi.yml
- filename: threatconnect-batch-api-openapi.yml
  format: yaml
  label: ThreatConnect Batch API
  slug: threatconnect-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatconnect/refs/heads/main/openapi/threatconnect-batch-api-openapi.yml
- filename: threatconnect-cases-api-openapi.yml
  format: yaml
  label: ThreatConnect Cases API
  slug: threatconnect-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatconnect/refs/heads/main/openapi/threatconnect-cases-api-openapi.yml
- filename: threatconnect-custommetrics-api-openapi.yml
  format: yaml
  label: ThreatConnect Custommetrics API
  slug: threatconnect-custommetrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatconnect/refs/heads/main/openapi/threatconnect-custommetrics-api-openapi.yml
- filename: threatconnect-groups-api-openapi.yml
  format: yaml
  label: ThreatConnect Groups API
  slug: threatconnect-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatconnect/refs/heads/main/openapi/threatconnect-groups-api-openapi.yml
- filename: threatconnect-indicators-api-openapi.yml
  format: yaml
  label: ThreatConnect Indicators API
  slug: threatconnect-indicators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatconnect/refs/heads/main/openapi/threatconnect-indicators-api-openapi.yml
- filename: threatconnect-notes-api-openapi.yml
  format: yaml
  label: ThreatConnect Notes API
  slug: threatconnect-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatconnect/refs/heads/main/openapi/threatconnect-notes-api-openapi.yml
- filename: threatconnect-notifications-api-openapi.yml
  format: yaml
  label: ThreatConnect Notifications API
  slug: threatconnect-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatconnect/refs/heads/main/openapi/threatconnect-notifications-api-openapi.yml
- filename: threatconnect-services-api-openapi.yml
  format: yaml
  label: ThreatConnect Services API
  slug: threatconnect-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatconnect/refs/heads/main/openapi/threatconnect-services-api-openapi.yml
- filename: threatconnect-tasks-api-openapi.yml
  format: yaml
  label: ThreatConnect Tasks API
  slug: threatconnect-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatconnect/refs/heads/main/openapi/threatconnect-tasks-api-openapi.yml
- filename: threatconnect-tc-taxii-api-openapi.yml
  format: yaml
  label: ThreatConnect Tc Taxii API
  slug: threatconnect-tc-taxii-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatconnect/refs/heads/main/openapi/threatconnect-tc-taxii-api-openapi.yml
- filename: threatconnect-threatconnect-api-api-openapi.yml
  format: yaml
  label: ThreatConnect ThreatConnect API
  slug: threatconnect-threatconnect-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatconnect/refs/heads/main/openapi/threatconnect-threatconnect-api-api-openapi.yml
- filename: threatconnect-token-api-openapi.yml
  format: yaml
  label: ThreatConnect Token API
  slug: threatconnect-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatconnect/refs/heads/main/openapi/threatconnect-token-api-openapi.yml
- filename: threatconnect-types-api-openapi.yml
  format: yaml
  label: ThreatConnect Types API
  slug: threatconnect-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatconnect/refs/heads/main/openapi/threatconnect-types-api-openapi.yml
- filename: threatconnect-victims-api-openapi.yml
  format: yaml
  label: ThreatConnect Victims API
  slug: threatconnect-victims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatconnect/refs/heads/main/openapi/threatconnect-victims-api-openapi.yml
auth_types: []
description: Authentication methods for ThreatConnect API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Threatconnect Authentication
name_suffix: Authentication
oauth_flows: []
overview: ThreatConnect declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ThreatConnect
provider_slug: threatconnect
scheme_count: 2
schemes:
- evidence: The value of the Authorization header must be in the format TC-Token $API_TOKEN , where $API_TOKEN is the value of your API token.
  header: Authorization
  how_to_obtain: Generate an API token via the ThreatConnect UI (Org Settings → Create API User or Edit API User and click GENERATE TOKEN).
  location: header
  name: TC-Token
  type: apiKey
- evidence: HMAC authorization is typically only used for running Apps outside the ThreatConnect platform. Generation of the authorization headers when using HMAC will utilize the api_access_id and api_secret_key arguments.
  how_to_obtain: Provide the API Access ID and API Secret Key in the install.json configuration file.
  location: header
  name: HMAC
  type: hmac
slug: threatconnect-authentication
source_filename: threatconnect-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.threatconnect.com/en/latest/tcex/authorization.html
source_yaml: "generated: '2026-10-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.threatconnect.com/en/latest/tcex/authorization.html\nsources:\n- https://docs.threatconnect.com/en/latest/tcex/authorization.html\n- https://docs.threatconnect.com/en/latest/getting_started.html\n- https://docs.threatconnect.com/en/latest/rest_api/quick_start.html\n- https://docs.threatconnect.com/en/latest/python/quick_start.html\ndescription: Authentication methods for ThreatConnect API\nschemes:\n- type: apiKey\n  name: TC-Token\n  evidence: The value of the Authorization header must be in the format TC-Token $API_TOKEN , where $API_TOKEN is the value of your API token.\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an API token via the ThreatConnect UI (Org Settings → Create API User or Edit API User and click GENERATE TOKEN).\n- type: hmac\n  name: HMAC\n  evidence: HMAC authorization is typically only used for running Apps outside the\
  \ ThreatConnect platform. Generation of the authorization headers\n    when using HMAC will utilize the api_access_id and api_secret_key arguments.\n  location: header\n  how_to_obtain: Provide the API Access ID and API Secret Key in the install.json configuration file.\ndocs: https://docs.threatconnect.com/en/latest/tcex/authorization.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/threatconnect/refs/heads/main/authentication/threatconnect-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Cybersecurity
- Threat Intelligence
- Security Operations
- Platform
---
