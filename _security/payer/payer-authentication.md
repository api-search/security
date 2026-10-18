---
anonymous_access: false
api_key_in: []
api_specs:
- filename: payer-all-api-openapi.yml
  format: yaml
  label: Payer All API
  slug: payer-all-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/openapi/payer-all-api-openapi.yml
- filename: payer-audit-api-openapi.yml
  format: yaml
  label: Payer Audit API
  slug: payer-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/openapi/payer-audit-api-openapi.yml
- filename: payer-changelog-api-openapi.yml
  format: yaml
  label: Payer Changelog API
  slug: payer-changelog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/openapi/payer-changelog-api-openapi.yml
- filename: payer-documentation-api-openapi.yml
  format: yaml
  label: Payer Documentation API
  slug: payer-documentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/openapi/payer-documentation-api-openapi.yml
- filename: payer-events-api-openapi.yml
  format: yaml
  label: Payer Events API
  slug: payer-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/openapi/payer-events-api-openapi.yml
- filename: payer-export-api-openapi.yml
  format: yaml
  label: Payer Export API
  slug: payer-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/openapi/payer-export-api-openapi.yml
- filename: payer-invoices-api-openapi.yml
  format: yaml
  label: Payer Invoices API
  slug: payer-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/openapi/payer-invoices-api-openapi.yml
- filename: payer-oauth2-api-openapi.yml
  format: yaml
  label: Payer Oauth2 API
  slug: payer-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/openapi/payer-oauth2-api-openapi.yml
- filename: payer-orders-api-openapi.yml
  format: yaml
  label: Payer Orders API
  slug: payer-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/openapi/payer-orders-api-openapi.yml
- filename: payer-page-api-openapi.yml
  format: yaml
  label: Payer Page API
  slug: payer-page-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/openapi/payer-page-api-openapi.yml
- filename: payer-payer-api-api-openapi.yml
  format: yaml
  label: Payer Payer API
  slug: payer-payer-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/openapi/payer-payer-api-api-openapi.yml
- filename: payer-reader-access-api-openapi.yml
  format: yaml
  label: Payer Reader Access API
  slug: payer-reader-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/openapi/payer-reader-access-api-openapi.yml
- filename: payer-reference-api-openapi.yml
  format: yaml
  label: Payer Reference API
  slug: payer-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/openapi/payer-reference-api-openapi.yml
- filename: payer-search-api-openapi.yml
  format: yaml
  label: Payer Search API
  slug: payer-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/openapi/payer-search-api-openapi.yml
- filename: payer-users-api-openapi.yml
  format: yaml
  label: Payer Users API
  slug: payer-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/openapi/payer-users-api-openapi.yml
- filename: payer-version-api-openapi.yml
  format: yaml
  label: Payer Version API
  slug: payer-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/openapi/payer-version-api-openapi.yml
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
- Fintech
- Automation
---
