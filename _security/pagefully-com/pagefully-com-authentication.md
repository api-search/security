---
anonymous_access: false
api_key_in: []
api_specs:
- filename: pagefully-com-openapi-generated.yml
  format: yaml
  label: Pagefully API
  slug: pagefully-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagefully-com/openapi/_ae-authored/pagefully-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Pagefully Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pagefully declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Pagefully
provider_slug: pagefully-com
scheme_count: 1
schemes:
- evidence: The key lets Pagefully read your keyword field and send a page to App Store Connect.
  header: Authorization
  how_to_obtain: Generate a Team key with the App Manager role in App Store Connect, then copy the Issuer ID, Key ID, and upload the private key file.
  location: header
  name: App Store Connect API key
  type: jwt
slug: pagefully-com-authentication
source_filename: pagefully-com-authentication.yml
source_heading: Authentication Profile
source_url: https://pagefully.com/help/using-pagefully/preview-pages-for-your-app
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://pagefully.com/help/using-pagefully/preview-pages-for-your-app\nsources:\n- https://pagefully.com/help/using-pagefully/preview-pages-for-your-app\n- https://pagefully.com/help/getting-started/what-is-pagefully\n- https://pagefully.com/help/getting-started/quick-start\n- https://pagefully.com/help/getting-started/how-pagefully-works\nschemes:\n- type: jwt\n  name: App Store Connect API key\n  evidence: The key lets Pagefully read your keyword field and send a page to App Store Connect.\n  location: header\n  header: Authorization\n  how_to_obtain: Generate a Team key with the App Manager role in App Store Connect, then copy the Issuer ID, Key ID, and upload the private key\n    file.\ndocs: https://pagefully.com/help/using-pagefully/preview-pages-for-your-app\n"
source_yaml_url: https://artifacts.apis.io/pagefully-com/authentication/pagefully-com-authentication.yml
summary_line: 1 scheme
tags:
- Mobile
- App Store
- Marketing
- iOS
- Custom Pages
---
