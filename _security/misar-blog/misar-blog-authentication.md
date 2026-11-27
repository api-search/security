---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Misar.Blog products (MisarDev and MisarMail).
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Misar.Blog Authentication
name_suffix: Authentication
oauth_flows: []
overview: Misar.Blog declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Misar.Blog
provider_slug: misar-blog
scheme_count: 1
schemes:
- evidence: 'Send the key in the Authorization header as a Bearer token: curl https://api.misar.io/dev/v1/projects \ -H "Authorization: Bearer mdk_YOUR_KEY_HERE"'
  header: Authorization
  how_to_obtain: Create a key in the MisarDev dashboard Settings → API Keys and copy the secret (starts with mdk_).
  location: header
  name: MisarDev API Key
  type: apiKey
slug: misar-blog-authentication
source_filename: misar-blog-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.misar.io/dev/api-reference/authentication
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.misar.io/dev/api-reference/authentication\nsources:\n- https://docs.misar.io/dev/api-reference/authentication\n- https://docs.misar.io/mail/getting-started/authentication\n- https://docs.misar.io/mail/api-reference/authentication\n- https://docs.misar.io/mail/api-reference/api-keys\ndescription: Authentication methods for Misar.Blog products (MisarDev and MisarMail).\nschemes:\n- type: apiKey\n  name: MisarDev API Key\n  evidence: 'Send the key in the Authorization header as a Bearer token: curl https://api.misar.io/dev/v1/projects \\ -H \"Authorization: Bearer\n    mdk_YOUR_KEY_HERE\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in the MisarDev dashboard Settings → API Keys and copy the secret (starts with mdk_).\ndocs: https://docs.misar.io/dev/api-reference/authentication\nnote: 2 extracted row(s) were dropped because their quote was\
  \ not on the page.\n"
source_yaml_url: https://artifacts.apis.io/misar-blog/authentication/misar-blog-authentication.yml
summary_line: 1 scheme
tags:
- Blogging
- Artificial Intelligence
- Content Creation
- Platform
- Free
---
