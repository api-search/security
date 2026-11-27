---
anonymous_access: false
api_key_in: []
api_specs:
- filename: terminal-telematics-applications-api-openapi.yml
  format: yaml
  label: Terminal Applications API
  slug: terminal-telematics-applications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal-telematics/openapi/terminal-telematics-applications-api-openapi.yml
- filename: terminal-telematics-authentication-api-openapi.yml
  format: yaml
  label: Terminal Authentication API
  slug: terminal-telematics-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal-telematics/openapi/terminal-telematics-authentication-api-openapi.yml
- filename: terminal-telematics-connections-api-openapi.yml
  format: yaml
  label: Terminal Connections API
  slug: terminal-telematics-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal-telematics/openapi/terminal-telematics-connections-api-openapi.yml
- filename: terminal-telematics-data-management-api-openapi.yml
  format: yaml
  label: Terminal Data Management API
  slug: terminal-telematics-data-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal-telematics/openapi/terminal-telematics-data-management-api-openapi.yml
- filename: terminal-telematics-devices-api-openapi.yml
  format: yaml
  label: Terminal Devices API
  slug: terminal-telematics-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal-telematics/openapi/terminal-telematics-devices-api-openapi.yml
- filename: terminal-telematics-drivers-api-openapi.yml
  format: yaml
  label: Terminal Drivers API
  slug: terminal-telematics-drivers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal-telematics/openapi/terminal-telematics-drivers-api-openapi.yml
- filename: terminal-telematics-fault-codes-api-openapi.yml
  format: yaml
  label: Terminal Fault Codes API
  slug: terminal-telematics-fault-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal-telematics/openapi/terminal-telematics-fault-codes-api-openapi.yml
- filename: terminal-telematics-groups-api-openapi.yml
  format: yaml
  label: Terminal Groups API
  slug: terminal-telematics-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal-telematics/openapi/terminal-telematics-groups-api-openapi.yml
- filename: terminal-telematics-hours-of-service-api-openapi.yml
  format: yaml
  label: Terminal Hours of Service API
  slug: terminal-telematics-hours-of-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal-telematics/openapi/terminal-telematics-hours-of-service-api-openapi.yml
- filename: terminal-telematics-ifta-api-openapi.yml
  format: yaml
  label: Terminal IFTA API
  slug: terminal-telematics-ifta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal-telematics/openapi/terminal-telematics-ifta-api-openapi.yml
- filename: terminal-telematics-issues-api-openapi.yml
  format: yaml
  label: Terminal Issues API
  slug: terminal-telematics-issues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal-telematics/openapi/terminal-telematics-issues-api-openapi.yml
- filename: terminal-telematics-link-api-openapi.yml
  format: yaml
  label: Terminal Link API
  slug: terminal-telematics-link-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal-telematics/openapi/terminal-telematics-link-api-openapi.yml
- filename: terminal-telematics-providers-api-openapi.yml
  format: yaml
  label: Terminal Providers API
  slug: terminal-telematics-providers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal-telematics/openapi/terminal-telematics-providers-api-openapi.yml
- filename: terminal-telematics-safety-api-openapi.yml
  format: yaml
  label: Terminal Safety API
  slug: terminal-telematics-safety-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal-telematics/openapi/terminal-telematics-safety-api-openapi.yml
- filename: terminal-telematics-trailers-api-openapi.yml
  format: yaml
  label: Terminal Trailers API
  slug: terminal-telematics-trailers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal-telematics/openapi/terminal-telematics-trailers-api-openapi.yml
- filename: terminal-telematics-trips-api-openapi.yml
  format: yaml
  label: Terminal Trips API
  slug: terminal-telematics-trips-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal-telematics/openapi/terminal-telematics-trips-api-openapi.yml
- filename: terminal-telematics-usage-api-openapi.yml
  format: yaml
  label: Terminal Usage API
  slug: terminal-telematics-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal-telematics/openapi/terminal-telematics-usage-api-openapi.yml
- filename: terminal-telematics-vehicle-utilization-api-openapi.yml
  format: yaml
  label: Terminal Vehicle Utilization API
  slug: terminal-telematics-vehicle-utilization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal-telematics/openapi/terminal-telematics-vehicle-utilization-api-openapi.yml
- filename: terminal-telematics-vehicles-api-openapi.yml
  format: yaml
  label: Terminal Vehicles API
  slug: terminal-telematics-vehicles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/terminal-telematics/openapi/terminal-telematics-vehicles-api-openapi.yml
auth_types: []
description: Authentication methods for Terminal API and provider OAuth integrations.
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Terminal Authentication
name_suffix: Authentication
oauth_flows: []
overview: Terminal declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Terminal
provider_slug: terminal-telematics
scheme_count: 4
schemes:
- evidence: Your publishable key is used for client-side authentication from web browsers and mobile applications through the consent flow.
  header: Authorization
  how_to_obtain: Get your publishable key from the Dashboard.
  location: header
  name: Publishable Key
  type: apiKey
- evidence: Secret keys are used for server-side authentication and provide full access to Terminal's backend APIs.
  header: Authorization
  how_to_obtain: Get your secret key from the Dashboard.
  location: header
  name: Secret Key
  type: apiKey
- evidence: 'To establish an OAuth client with Motive, execute the following steps:'
  how_to_obtain: Create an OAuth application in the Motive Developer Portal and paste the Client ID and Client Secret into the Terminal dashboard.
  name: Motive OAuth
  scopes:
  - Company Details (Read Only)
  - Vehicles (Read Only)
  - ELDs (Read Only)
  - Groups (Read Only)
  - Drivers and Fleet Managers (Read Only)
  - Fault Codes (Read Only)
  - Vehicles with Current Location and Current Driver (Read Only)
  - Drivers with Current Location and Current Vehicle (Read Only)
  - Vehicle Location History (Read Only)
  - Assets (Read Only)
  - Asset with Asset Gateway Location History (Read Only)
  - Drivers with Hours of Service (Read Only)
  - HOS Logs (Read Only)
  - Speeding Events (Read Only)
  - Scorecard Summary (Read Only)
  - IFTA Trip Reports (Read Only)
  - Vehicles' Mileage Summary (Read Only)
  - Utilization Summary by Vehicle (Read Only)
  type: oauth2
- evidence: 'To create an OAuth application with Samsara, follow these steps:'
  how_to_obtain: Create an OAuth application in the Samsara dashboard, add the redirect URL, select scopes, then paste the Client ID and Client Secret into the Terminal dashboard.
  name: Samsara OAuth
  scopes:
  - Setup & Administration > Read Org Information
  - Setup & Administration > Read Webhooks
  - Setup & Administration > Write Webhooks
  - Vehicles > Read Vehicles
  - Setup & Administration > Read Tags
  - Setup & Administration > Read Gateways
  - Drivers > Read Drivers
  - Vehicles > Read Vehicle Statistics
  - Assignments > Read Assignments
  - Vehicles > Read Vehicle Trips
  - Trailers > Read Trailers
  - Equipment > Read Equipment
  - Trailers > Read Trailer Statistics
  - Equipment > Read Equipment Statistics
  - Compliance > Read ELD Hours of Service
  - Compliance > Read ELD Compliance Settings
  - Safety & Cameras > Read Safety Events & Scores
  - Safety & Cameras > Read Camera Media
  - Speeding Intervals > Read Speeding Intervals
  - Compliance > Read IFTA (US)
  type: oauth2
slug: terminal-telematics-authentication
source_filename: terminal-telematics-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.withterminal.com/guides/motive-oauth-configuration.md
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.withterminal.com/guides/motive-oauth-configuration.md\nsources:\n- https://docs.withterminal.com/guides/motive-oauth-configuration.md\n- https://docs.withterminal.com/guides/samsara-oauth-configuration.md\n- https://docs.withterminal.com/api-reference/authentication.md\n- https://docs.withterminal.com/api-reference/authentication/public-token-exchange.md\ndescription: Authentication methods for Terminal API and provider OAuth integrations.\nschemes:\n- type: apiKey\n  name: Publishable Key\n  evidence: Your publishable key is used for client-side authentication from web browsers and mobile applications through the consent flow.\n  location: header\n  header: Authorization\n  how_to_obtain: Get your publishable key from the Dashboard.\n- type: apiKey\n  name: Secret Key\n  evidence: Secret keys are used for server-side authentication and provide full access to Terminal's\
  \ backend APIs.\n  location: header\n  header: Authorization\n  how_to_obtain: Get your secret key from the Dashboard.\n- type: oauth2\n  name: Motive OAuth\n  evidence: 'To establish an OAuth client with Motive, execute the following steps:'\n  scopes:\n  - Company Details (Read Only)\n  - Vehicles (Read Only)\n  - ELDs (Read Only)\n  - Groups (Read Only)\n  - Drivers and Fleet Managers (Read Only)\n  - Fault Codes (Read Only)\n  - Vehicles with Current Location and Current Driver (Read Only)\n  - Drivers with Current Location and Current Vehicle (Read Only)\n  - Vehicle Location History (Read Only)\n  - Assets (Read Only)\n  - Asset with Asset Gateway Location History (Read Only)\n  - Drivers with Hours of Service (Read Only)\n  - HOS Logs (Read Only)\n  - Speeding Events (Read Only)\n  - Scorecard Summary (Read Only)\n  - IFTA Trip Reports (Read Only)\n  - Vehicles' Mileage Summary (Read Only)\n  - Utilization Summary by Vehicle (Read Only)\n  how_to_obtain: Create an OAuth application\
  \ in the Motive Developer Portal and paste the Client ID and Client Secret into the Terminal dashboard.\n- type: oauth2\n  name: Samsara OAuth\n  evidence: 'To create an OAuth application with Samsara, follow these steps:'\n  scopes:\n  - Setup & Administration > Read Org Information\n  - Setup & Administration > Read Webhooks\n  - Setup & Administration > Write Webhooks\n  - Vehicles > Read Vehicles\n  - Setup & Administration > Read Tags\n  - Setup & Administration > Read Gateways\n  - Drivers > Read Drivers\n  - Vehicles > Read Vehicle Statistics\n  - Assignments > Read Assignments\n  - Vehicles > Read Vehicle Trips\n  - Trailers > Read Trailers\n  - Equipment > Read Equipment\n  - Trailers > Read Trailer Statistics\n  - Equipment > Read Equipment Statistics\n  - Compliance > Read ELD Hours of Service\n  - Compliance > Read ELD Compliance Settings\n  - Safety & Cameras > Read Safety Events & Scores\n  - Safety & Cameras > Read Camera Media\n  - Speeding Intervals > Read Speeding Intervals\n\
  \  - Compliance > Read IFTA (US)\n  how_to_obtain: Create an OAuth application in the Samsara dashboard, add the redirect URL, select scopes, then paste the Client ID and Client\n    Secret into the Terminal dashboard.\ndocs: https://docs.withterminal.com/guides/motive-oauth-configuration.md\n"
source_yaml_url: https://artifacts.apis.io/terminal-telematics/authentication/terminal-telematics-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Telematics
- Data
- Fleet Management
- Insurance
---
