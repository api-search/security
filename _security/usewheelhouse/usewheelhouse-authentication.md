---
anonymous_access: false
api_key_in: []
api_specs:
- filename: usewheelhouse-openapi-generated.yml
  format: yaml
  label: Wheelhouse API
  slug: usewheelhouse-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usewheelhouse/openapi/_ae-authored/usewheelhouse-openapi-generated.yml
auth_types: []
description: Wheelhouse RM API uses a single API key sent in the X-Integration-Api-Key header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Wheelhouse Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wheelhouse declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Wheelhouse
provider_slug: usewheelhouse
scheme_count: 1
schemes:
- evidence: For HTTP integrations that call the RM API directly, send an RM API key in the X-Integration-Api-Key header.
  header: X-Integration-Api-Key
  how_to_obtain: Generate in Wheelhouse account under API & MCP → API Keys (see Getting Started page).
  location: header
  name: Integration API Key
  type: apiKey
slug: usewheelhouse-authentication
source_filename: usewheelhouse-authentication.yml
source_heading: Authentication Profile
source_url: https://help.usewheelhouse.com/en/articles/17771409-managing-your-integration-api-keys-for-channel-partners.md
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://help.usewheelhouse.com/en/articles/17771409-managing-your-integration-api-keys-for-channel-partners.md\nsources:\n- https://help.usewheelhouse.com/en/articles/17771409-managing-your-integration-api-keys-for-channel-partners.md\n- https://docs.usewheelhouse.com/rm/authentication\n- https://help.usewheelhouse.com/en/articles/15468234-getting-started-with-the-wheelhouse-rm-api.md\ndescription: Wheelhouse RM API uses a single API key sent in the X-Integration-Api-Key header.\nschemes:\n- type: apiKey\n  name: Integration API Key\n  evidence: For HTTP integrations that call the RM API directly, send an RM API key in the X-Integration-Api-Key header.\n  location: header\n  header: X-Integration-Api-Key\n  how_to_obtain: Generate in Wheelhouse account under API & MCP → API Keys (see Getting Started page).\nnote: OAuth is mentioned for MCP server usage, but no token or authorize\
  \ URLs are provided on the pages.\ndocs: https://help.usewheelhouse.com/en/articles/17771409-managing-your-integration-api-keys-for-channel-partners.md\n"
source_yaml_url: https://artifacts.apis.io/usewheelhouse/authentication/usewheelhouse-authentication.yml
summary_line: 1 scheme
tags:
- Revenue Management
- Short-Term Rental
- Mid-Term Rentals
- Pricing API
- Analytics
---
