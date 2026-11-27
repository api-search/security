---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Proxmint
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Proxmint Authentication
name_suffix: Authentication
oauth_flows: []
overview: Proxmint declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Proxmint
provider_slug: proxmint
scheme_count: 2
schemes:
- evidence: Every product you buy has its own username and password. Both are on the product's page in your dashboard , with copy buttons.
  how_to_obtain: Credentials are shown on the product’s page in the dashboard after purchase.
  location: proxy URL
  name: Proxy username/password
  type: http-basic
- evidence: Create a key under Settings in the dashboard and send it as a bearer token.
  header: Authorization
  how_to_obtain: Generate a key in the Settings section of the dashboard; keys start with pmk_.
  location: header
  name: Customer API key
  type: http-bearer
slug: proxmint-authentication
source_filename: proxmint-authentication.yml
source_heading: Authentication Profile
source_url: https://proxmint.com/docs/quickstart
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://proxmint.com/docs/quickstart\nsources:\n- https://proxmint.com/docs/quickstart\n- https://proxmint.com/docs/api\ndescription: Authentication methods for Proxmint\nschemes:\n- type: http-basic\n  name: Proxy username/password\n  evidence: Every product you buy has its own username and password. Both are on the product's page in your dashboard , with copy buttons.\n  location: proxy URL\n  how_to_obtain: Credentials are shown on the product’s page in the dashboard after purchase.\n- type: http-bearer\n  name: Customer API key\n  evidence: Create a key under Settings in the dashboard and send it as a bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: Generate a key in the Settings section of the dashboard; keys start with pmk_.\ndocs: https://proxmint.com/docs/quickstart\n"
source_yaml_url: https://artifacts.apis.io/proxmint/authentication/proxmint-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Proxy
- Web Scraping
- Billing
- Geo-Targeting
---
