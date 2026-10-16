---
anonymous_access: false
api_key_in: []
api_specs:
- filename: payer-openapi-generated.yml
  format: yaml
  label: Payer API
  slug: payer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/openapi/_ae-authored/payer-openapi-generated.yml
auth_types: []
description: Authentication schemes for Payer API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Payer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Payer declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Payer
provider_slug: payer
scheme_count: 2
schemes:
- evidence: 'curl --request POST \    --url https://api.developerhub.io/api/v1/version/50/reference \    --header "X-Api-Key: 689bbce8acc68b7a4346acca6a028e6f8126eb792b19a334f8e3f2a12ca8f561"'
  header: X-Api-Key
  how_to_obtain: Create an API Key in Project Settings → API Keys and copy it.
  location: header
  name: X-Api-Key
  type: apiKey
- evidence: 'curl --request POST \ --url ''https://b2b.payer.se/api/v3/invoices'' \ --header ''Authorization: Bearer {token}'' \ --data ''{ ... }'''
  header: Authorization
  how_to_obtain: Obtain a bearer token from Payer's authentication endpoint (not documented on the provided pages).
  location: header
  name: Authorization
  type: http-bearer
slug: payer-authentication
source_filename: payer-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.developerhub.io/support-center/api-key.md
source_yaml: "generated: '2026-10-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.developerhub.io/support-center/api-key.md\nsources:\n- https://docs.developerhub.io/support-center/api-key.md\n- https://docs.developerhub.io/api\n- https://docs.developerhub.io/support-center/getting-started.md\n- https://payerdocs.developerhub.io/payer-docs/b2b-invoicing---quickstart\ndescription: Authentication schemes for Payer API\nschemes:\n- type: apiKey\n  name: X-Api-Key\n  evidence: 'curl --request POST \\    --url https://api.developerhub.io/api/v1/version/50/reference \\    --header \"X-Api-Key: 689bbce8acc68b7a4346acca6a028e6f8126eb792b19a334f8e3f2a12ca8f561\"'\n  location: header\n  header: X-Api-Key\n  how_to_obtain: Create an API Key in Project Settings → API Keys and copy it.\n- type: http-bearer\n  name: Authorization\n  evidence: 'curl --request POST \\ --url ''https://b2b.payer.se/api/v3/invoices'' \\ --header ''Authorization: Bearer {token}'' \\\
  \ --data ''{ ...\n    }'''\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain a bearer token from Payer's authentication endpoint (not documented on the provided pages).\ndocs: https://docs.developerhub.io/support-center/api-key.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/authentication/payer-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Payments
- B2B
- FinTech
- Automation
---
