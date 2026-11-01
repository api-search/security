---
anonymous_access: false
api_key_in: []
api_specs:
- filename: adscrawl-browser-tasks-api-openapi.yml
  format: yaml
  label: AdsCrawl Browser tasks API
  slug: adscrawl-browser-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adscrawl/openapi/adscrawl-browser-tasks-api-openapi.yml
- filename: adscrawl-cloud-browsers-api-openapi.yml
  format: yaml
  label: AdsCrawl Cloud browsers API
  slug: adscrawl-cloud-browsers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adscrawl/openapi/adscrawl-cloud-browsers-api-openapi.yml
- filename: adscrawl-remote-cdp-api-openapi.yml
  format: yaml
  label: AdsCrawl Remote CDP API
  slug: adscrawl-remote-cdp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adscrawl/openapi/adscrawl-remote-cdp-api-openapi.yml
auth_types: []
description: Authentication methods for AdsCrawl API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Adscrawl Authentication
name_suffix: Authentication
oauth_flows: []
overview: AdsCrawl declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: AdsCrawl
provider_slug: adscrawl
scheme_count: 2
schemes:
- evidence: Pass your API key in the `x-api-key` header on every request.
  header: x-api-key
  how_to_obtain: Copy your API key from the dashboard keys section.
  location: header
  name: API Key
  type: apiKey
- evidence: 'Cloud browser list, create, launch, start, and stop endpoints also accept a session JWT in the `Authorization: Bearer <SESSION_JWT>` header.'
  header: Authorization
  how_to_obtain: Obtain a session JWT from a logged‑in dashboard session.
  location: header
  name: Session JWT
  type: http-bearer
slug: adscrawl-authentication
source_filename: adscrawl-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.adscrawl.net/authentication.md
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.adscrawl.net/authentication.md\nsources:\n- https://docs.adscrawl.net/authentication.md\n- https://docs.adscrawl.net/api-reference/cdp-live-token.md\n- https://docs.adscrawl.net/quickstart.md\ndescription: Authentication methods for AdsCrawl API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: Pass your API key in the `x-api-key` header on every request.\n  location: header\n  header: x-api-key\n  how_to_obtain: Copy your API key from the dashboard keys section.\n- type: http-bearer\n  name: Session JWT\n  evidence: 'Cloud browser list, create, launch, start, and stop endpoints also accept a session JWT in the `Authorization: Bearer <SESSION_JWT>`\n    header.'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain a session JWT from a logged‑in dashboard session.\nnote: No OAuth2 flows are documented for AdsCrawl. 1 extracted row(s) were dropped\
  \ because their quote was not on the page.\ndocs: https://docs.adscrawl.net/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/adscrawl/authentication/adscrawl-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Browser Automation
- WebDataExtraction
- Playwright
- Puppeteer
- Chrome DevTools Protocol
---
