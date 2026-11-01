---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for BI.P.EYE API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Bipeye Authentication
name_suffix: Authentication
oauth_flows: []
overview: BIPEYE declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: BIPEYE
provider_slug: bipeye
scheme_count: 1
schemes:
- evidence: Every endpoint requires your organization API key in the X-API-Key header.
  header: X-API-Key
  how_to_obtain: Generate one on the OpenAPI > API Keys page in BI.P.EYE.
  location: header
  name: X-API-Key
  type: apiKey
slug: bipeye-authentication
source_filename: bipeye-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.bipeye.com/product-docs/overview/embed-dashboards/embed-dashboards-restriced-data-per-api-key.md
source_yaml: "generated: '2026-10-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.bipeye.com/product-docs/overview/embed-dashboards/embed-dashboards-restriced-data-per-api-key.md\nsources:\n- https://docs.bipeye.com/product-docs/overview/embed-dashboards/embed-dashboards-restriced-data-per-api-key.md\n- https://docs.bipeye.com/product-docs/overview/openapi/authentication.md\n- https://docs.bipeye.com/product-docs/overview/credentials.md\n- https://docs.bipeye.com/product-docs/overview/credentials/databases.md\ndescription: Authentication schemes for BI.P.EYE API\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: Every endpoint requires your organization API key in the X-API-Key header.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Generate one on the OpenAPI > API Keys page in BI.P.EYE.\ndocs: https://docs.bipeye.com/product-docs/overview/embed-dashboards/embed-dashboards-restriced-data-per-api-key.md\n"
source_yaml_url: https://artifacts.apis.io/bipeye/authentication/bipeye-authentication.yml
summary_line: 1 scheme
tags:
- Company
---
