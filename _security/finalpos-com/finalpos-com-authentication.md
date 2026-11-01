---
anonymous_access: false
api_key_in: []
auth_types: []
description: Final POS API uses API keys passed in request headers.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Finalpos Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: finalpos-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: finalpos-com
provider_slug: finalpos-com
scheme_count: 2
schemes:
- evidence: Use a company key in the x-api-key header for standard resource endpoints, or an organization key in the x-org-api-key header for org-level company management.
  header: x-api-key
  how_to_obtain: Create a company API key under Settings > API Keys in manage.finalpos.com or scale.finalpos.com.
  location: header
  name: Company API key
  type: apiKey
- evidence: Use a company key in the x-api-key header for standard resource endpoints, or an organization key in the x-org-api-key header for org-level company management.
  header: x-org-api-key
  how_to_obtain: Create an organization API key under Settings > API Keys in manage.finalpos.com or scale.finalpos.com.
  location: header
  name: Organization API key
  type: apiKey
slug: finalpos-com-authentication
source_filename: finalpos-com-authentication.yml
source_heading: Authentication Profile
source_url: https://finalpos.com/docs/authentication
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://finalpos.com/docs/authentication\nsources:\n- https://finalpos.com/docs/authentication\n- https://finalpos.com/docs/authentication.md\n- https://finalpos.com/blog/station-home-phase-2-quick-payments-flow-switching-and-better-peripheral-setup\n- https://finalpos.com/blog/first-week-on-a-new-pos-setup-checklist\ndescription: Final POS API uses API keys passed in request headers.\nschemes:\n- type: apiKey\n  name: Company API key\n  evidence: Use a company key in the x-api-key header for standard resource endpoints, or an organization key in the x-org-api-key header for\n    org-level company management.\n  location: header\n  header: x-api-key\n  how_to_obtain: Create a company API key under Settings > API Keys in manage.finalpos.com or scale.finalpos.com.\n- type: apiKey\n  name: Organization API key\n  evidence: Use a company key in the x-api-key header for standard resource\
  \ endpoints, or an organization key in the x-org-api-key header for\n    org-level company management.\n  location: header\n  header: x-org-api-key\n  how_to_obtain: Create an organization API key under Settings > API Keys in manage.finalpos.com or scale.finalpos.com.\nnote: Each request must include exactly one of the two headers; sending both is rejected.\ndocs: https://finalpos.com/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/finalpos-com/authentication/finalpos-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- POS
- Retail
- Payments
- FinTech
---
