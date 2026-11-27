---
anonymous_access: false
api_key_in: []
api_specs:
- filename: equalweb-openapi-generated.yml
  format: yaml
  label: EqualWeb API
  slug: equalweb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/equalweb/openapi/_ae-authored/equalweb-openapi-generated.yml
auth_types: []
description: Authentication schemes for EqualWeb integrations
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: EqualWeb Authentication
name_suffix: Authentication
oauth_flows: []
overview: EqualWeb declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: EqualWeb
provider_slug: equalweb
scheme_count: 3
schemes:
- evidence: There is no cloud setup step. No app to register, no developer console, no keys to create on Shopify's side. The install itself creates the secure connection over Shopify's OAuth.
  flows:
  - authorization_code
  how_to_obtain: Install the EqualWeb app from your EqualWeb account; Shopify handles the OAuth flow and grants the app the listed scopes.
  name: Shopify OAuth
  scopes:
  - read_files
  - write_files
  type: oauth2
- evidence: 'In EqualWeb: Under Option 1 - API developer key, paste the Client ID and secret.'
  header: Authorization
  how_to_obtain: Create a developer key in Canvas (Admin → Developer Keys → + Developer Key → + API Key) and copy its Client ID and secret.
  location: header
  name: EqualWeb API key (Canvas option 1)
  type: apiKey
- evidence: 'In EqualWeb: Under Option 2 - access token, paste the token.'
  header: Authorization
  how_to_obtain: Generate a new access token in Canvas (Account → Settings → + New Access Token) and copy it.
  location: header
  name: Canvas access token (Option 2)
  type: apiKey
slug: equalweb-authentication
source_filename: equalweb-authentication.yml
source_heading: Authentication Profile
source_url: https://www.equalweb.com/platform/pdf_tools/integrations/shopify-setup.html
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.equalweb.com/platform/pdf_tools/integrations/shopify-setup.html\nsources:\n- https://www.equalweb.com/platform/pdf_tools/integrations/shopify-setup.html\n- https://www.equalweb.com/platform/pdf_tools/integrations/canvas-setup.html\n- https://www.equalweb.com/ai-business-assistant/guide/\ndescription: Authentication schemes for EqualWeb integrations\nschemes:\n- type: oauth2\n  name: Shopify OAuth\n  evidence: There is no cloud setup step. No app to register, no developer console, no keys to create on Shopify's side. The install itself creates\n    the secure connection over Shopify's OAuth.\n  flows:\n  - authorization_code\n  scopes:\n  - read_files\n  - write_files\n  how_to_obtain: Install the EqualWeb app from your EqualWeb account; Shopify handles the OAuth flow and grants the app the listed scopes.\n- type: apiKey\n  name: EqualWeb API key (Canvas option 1)\n \
  \ evidence: 'In EqualWeb: Under Option 1 - API developer key, paste the Client ID and secret.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a developer key in Canvas (Admin → Developer Keys → + Developer Key → + API Key) and copy its Client ID and secret.\n- type: apiKey\n  name: Canvas access token (Option 2)\n  evidence: 'In EqualWeb: Under Option 2 - access token, paste the token.'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate a new access token in Canvas (Account → Settings → + New Access Token) and copy it.\ndocs: https://www.equalweb.com/platform/pdf_tools/integrations/shopify-setup.html\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/equalweb/authentication/equalweb-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Accessibility
- Artificial Intelligence
- Compliance
- Software-as-a-Service
---
