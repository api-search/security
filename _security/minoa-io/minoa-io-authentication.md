---
anonymous_access: false
api_key_in: []
api_specs:
- filename: minoa-io-company-api-openapi.yml
  format: yaml
  label: Minoa Company API
  slug: minoa-io-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/minoa-io/openapi/minoa-io-company-api-openapi.yml
- filename: minoa-io-content-api-openapi.yml
  format: yaml
  label: Minoa Content API
  slug: minoa-io-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/minoa-io/openapi/minoa-io-content-api-openapi.yml
- filename: minoa-io-discovery-api-openapi.yml
  format: yaml
  label: Minoa Discovery API
  slug: minoa-io-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/minoa-io/openapi/minoa-io-discovery-api-openapi.yml
- filename: minoa-io-forms-api-openapi.yml
  format: yaml
  label: Minoa Forms API
  slug: minoa-io-forms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/minoa-io/openapi/minoa-io-forms-api-openapi.yml
- filename: minoa-io-pricing-api-openapi.yml
  format: yaml
  label: Minoa Pricing API
  slug: minoa-io-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/minoa-io/openapi/minoa-io-pricing-api-openapi.yml
auth_types: []
description: Authentication schemes for Minoa
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Minoa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Minoa declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Minoa
provider_slug: minoa-io
scheme_count: 1
schemes:
- evidence: Minoa provides a **Bearer token** for SCIM API authentication.
  header: Authorization
  how_to_obtain: Contact support to enable SCIM and receive a unique Bearer token for the organization.
  location: header
  name: SCIM Bearer Token
  type: http-bearer
slug: minoa-io-authentication
source_filename: minoa-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.minoa.io/pages/integrations/authentication/sso.md
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.minoa.io/pages/integrations/authentication/sso.md\nsources:\n- https://docs.minoa.io/pages/integrations/authentication/sso.md\n- https://docs.minoa.io/pages/integrations/authentication/scim.md\n- https://docs.minoa.io/pages/integrations/authentication/password.md\n- https://docs.minoa.io/pages/getting-started/introduction.md\ndescription: Authentication schemes for Minoa\nschemes:\n- type: http-bearer\n  name: SCIM Bearer Token\n  evidence: Minoa provides a **Bearer token** for SCIM API authentication.\n  location: header\n  header: Authorization\n  how_to_obtain: Contact support to enable SCIM and receive a unique Bearer token for the organization.\ndocs: https://docs.minoa.io/pages/integrations/authentication/sso.md\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/minoa-io/authentication/minoa-io-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Value-Intelligence
- Software-as-a-Service
- B2B
- Analytics
---
