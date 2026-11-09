---
anonymous_access: false
api_key_in: []
api_specs:
- filename: consentstack-io-openapi-generated.yml
  format: yaml
  label: ConsentStack API
  slug: consentstack-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/consentstack-io/openapi/_ae-authored/consentstack-io-openapi-generated.yml
auth_types: []
description: Authentication uses a site‑specific API key passed as a query parameter named “k” on the SDK script URLs.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Consentstack Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: ConsentStack declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ConsentStack
provider_slug: consentstack-io
scheme_count: 1
schemes:
- evidence: 'Add these three tags to your website''s <head> , replacing <YOUR_SITE_KEY> with the key from the previous step:'
  how_to_obtain: Generated per site in the ConsentStack dashboard; displayed on the site’s overview page.
  location: query
  name: Site Key
  type: apiKey
slug: consentstack-io-authentication
source_filename: consentstack-io-authentication.yml
source_heading: Authentication Profile
source_url: https://www.consentstack.io/docs/developers/theming-tokens
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.consentstack.io/docs/developers/theming-tokens\nsources:\n- https://www.consentstack.io/docs/developers/theming-tokens\n- https://www.consentstack.io/docs/getting-started\n- https://www.consentstack.io/docs/guides/testing-and-verification\ndescription: Authentication uses a site‑specific API key passed as a query parameter named “k” on the SDK script URLs.\nschemes:\n- type: apiKey\n  name: Site Key\n  evidence: 'Add these three tags to your website''s <head> , replacing <YOUR_SITE_KEY> with the key from the previous step:'\n  location: query\n  how_to_obtain: Generated per site in the ConsentStack dashboard; displayed on the site’s overview page.\nnote: No other authentication mechanisms (OAuth2, HTTP, etc.) are documented on the provided pages.\ndocs: https://www.consentstack.io/docs/developers/theming-tokens\n"
source_yaml_url: https://artifacts.apis.io/consentstack-io/authentication/consentstack-io-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Consent Management
- Privacy
- GDPR
- CCPA
- Cookie
---
