---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Audible Magic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Audible Magic declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Audible Magic
provider_slug: audible-magic
scheme_count: 3
schemes:
- description: Assigned value to identify requests made by partner, used in Fulfillment Content API
  in: query
  name: RetailerID
  type: apiKey
- description: Toolkit configuration file issued to customers for identification services
  in: file
  name: Configuration file
  type: apiKey
- description: HTTP GET with a cookie for Fulfillment Content API
  in: cookie
  name: Session cookie
  type: cookie
slug: audible-magic-authentication
source_filename: audible-magic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: searched\nsource: https://support.audiblemagic.com/how-does-the-audible-magic-fulfillment-api-work\nschemes:\n  - type: apiKey\n    name: RetailerID\n    description: Assigned value to identify requests made by partner, used in Fulfillment Content API\n    in: query\n  - type: apiKey\n    name: Configuration file\n    description: Toolkit configuration file issued to customers for identification services\n    in: file\n  - type: cookie\n    name: Session cookie\n    description: HTTP GET with a cookie for Fulfillment Content API\n    in: cookie\nnote: Authentication appears to be through customer-specific configuration files and retailer IDs rather than standard API keys or OAuth."
source_yaml_url: https://artifacts.apis.io/audible-magic/authentication/audible-magic-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Automatic Content Recognition
- Content Identification
- Rights Management
- Music Licensing
- Copyright Compliance
- Audio Fingerprinting
---
