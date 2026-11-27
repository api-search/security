---
anonymous_access: false
api_key_in: []
api_specs:
- filename: teslemetry-automations-api-openapi.yml
  format: yaml
  label: Teslemetry Automations API
  slug: teslemetry-automations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/teslemetry/openapi/teslemetry-automations-api-openapi.yml
- filename: teslemetry-charging-api-openapi.yml
  format: yaml
  label: Teslemetry Charging API
  slug: teslemetry-charging-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/teslemetry/openapi/teslemetry-charging-api-openapi.yml
- filename: teslemetry-energy-api-openapi.yml
  format: yaml
  label: Teslemetry Energy API
  slug: teslemetry-energy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/teslemetry/openapi/teslemetry-energy-api-openapi.yml
- filename: teslemetry-energy-command-api-openapi.yml
  format: yaml
  label: Teslemetry Energy Command API
  slug: teslemetry-energy-command-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/teslemetry/openapi/teslemetry-energy-command-api-openapi.yml
- filename: teslemetry-general-api-openapi.yml
  format: yaml
  label: Teslemetry General API
  slug: teslemetry-general-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/teslemetry/openapi/teslemetry-general-api-openapi.yml
- filename: teslemetry-meta-api-openapi.yml
  format: yaml
  label: Teslemetry Meta API
  slug: teslemetry-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/teslemetry/openapi/teslemetry-meta-api-openapi.yml
- filename: teslemetry-streaming-api-openapi.yml
  format: yaml
  label: Teslemetry Streaming API
  slug: teslemetry-streaming-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/teslemetry/openapi/teslemetry-streaming-api-openapi.yml
- filename: teslemetry-user-api-openapi.yml
  format: yaml
  label: Teslemetry User API
  slug: teslemetry-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/teslemetry/openapi/teslemetry-user-api-openapi.yml
- filename: teslemetry-vehicle-api-openapi.yml
  format: yaml
  label: Teslemetry Vehicle API
  slug: teslemetry-vehicle-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/teslemetry/openapi/teslemetry-vehicle-api-openapi.yml
- filename: teslemetry-vehicle-command-api-openapi.yml
  format: yaml
  label: Teslemetry Vehicle Command API
  slug: teslemetry-vehicle-command-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/teslemetry/openapi/teslemetry-vehicle-command-api-openapi.yml
- filename: teslemetry-vehicle-custom-commands-api-openapi.yml
  format: yaml
  label: Teslemetry Vehicle Custom Commands API
  slug: teslemetry-vehicle-custom-commands-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/teslemetry/openapi/teslemetry-vehicle-custom-commands-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Teslemetry Authentication
name_suffix: Authentication
oauth_flows: []
overview: Teslemetry declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Teslemetry
provider_slug: teslemetry
scheme_count: 2
schemes:
- evidence: Enter your access token from teslemetry.com/console
  header: Authorization
  how_to_obtain: Create an access token in the Teslemetry console (teslemetry.com/console).
  location: header
  name: Access Token
  type: http-bearer
- authorize_url: https://auth.tesla.com
  evidence: You sign in to both Teslemetry, and authorise your Tesla account by visiting teslemetry.com/login . This will redirect you to auth.tesla.com where you can enter your Tesla username, password, and two factor authentication (if enabled).
  how_to_obtain: Log in via teslemetry.com/login which redirects to auth.tesla.com to authorize the requested scopes.
  name: Tesla OAuth
  scopes:
  - Profile Info
  - Vehicle Information
  - Vehicle Location
  - Vehicle Commands
  - Vehicle Charging Management
  - Energy Product Information
  - Energy Product Commands
  type: oauth2
slug: teslemetry-authentication
source_filename: teslemetry-authentication.yml
source_heading: Authentication Profile
source_url: https://teslemetry.com/docs/n8n/credentials
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://teslemetry.com/docs/n8n/credentials\nsources:\n- https://teslemetry.com/docs/n8n/credentials\n- https://teslemetry.com/docs/topics/commandsigning\n- https://teslemetry.com/docs/getting-started/initial-setup\n- https://teslemetry.com/docs/getting-started/console\nschemes:\n- type: http-bearer\n  name: Access Token\n  evidence: Enter your access token from teslemetry.com/console\n  location: header\n  header: Authorization\n  how_to_obtain: Create an access token in the Teslemetry console (teslemetry.com/console).\n- type: oauth2\n  name: Tesla OAuth\n  evidence: You sign in to both Teslemetry, and authorise your Tesla account by visiting teslemetry.com/login . This will redirect you to auth.tesla.com\n    where you can enter your Tesla username, password, and two factor authentication (if enabled).\n  authorize_url: https://auth.tesla.com\n  scopes:\n  - Profile Info\n  -\
  \ Vehicle Information\n  - Vehicle Location\n  - Vehicle Commands\n  - Vehicle Charging Management\n  - Energy Product Information\n  - Energy Product Commands\n  how_to_obtain: Log in via teslemetry.com/login which redirects to auth.tesla.com to authorize the requested scopes.\ndocs: https://teslemetry.com/docs/n8n/credentials\n"
source_yaml_url: https://artifacts.apis.io/teslemetry/authentication/teslemetry-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Tesla
- Fleet API
- Home Automation
- Energy
---
