---
anonymous_access: false
api_key_in: []
api_specs:
- filename: avo-app-openapi-generated.yml
  format: yaml
  label: Avo API
  slug: avo-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/avo-app/openapi/_ae-authored/avo-app-openapi-generated.yml
auth_types: []
description: Authentication methods for Avo as documented
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Avo App Authentication
name_suffix: Authentication
oauth_flows: []
overview: Avo declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Avo
provider_slug: avo-app
scheme_count: 2
schemes:
- evidence: Avo API uses Basic authentication to authenticate requests with Avo service accounts.
  header: authorization
  how_to_obtain: Create a Service Account in workspace settings and generate a secret; use the Base64‑encoded "name:secret" as the value for the Authorization header with the "Basic" scheme.
  location: header
  name: Service Account Basic Auth
  type: http-basic
- evidence: Avo will sign each webhook call it sends to your endpoint by including a JWT token in each request authorization header.
  header: authorization
  how_to_obtain: Retrieve the unique secret key for the webhook from the Webhook publishing page in Avo; the JWT token is sent in the Authorization header as a Bearer token.
  location: header
  name: Webhook JWT Signature
  type: jwt
slug: avo-app-authentication
source_filename: avo-app-authentication.yml
source_heading: Authentication Profile
source_url: https://www.avo.app/docs/workspace-management/authentication
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.avo.app/docs/workspace-management/authentication\nsources:\n- https://www.avo.app/docs/workspace-management/authentication\n- https://www.avo.app/docs/reference/public-api/authentication\n- https://www.avo.app/docs/publishing/webhook-signing\n- https://www.avo.app/docs/index.md\ndescription: Authentication methods for Avo as documented\nschemes:\n- type: http-basic\n  name: Service Account Basic Auth\n  evidence: Avo API uses Basic authentication to authenticate requests with Avo service accounts.\n  location: header\n  header: authorization\n  how_to_obtain: Create a Service Account in workspace settings and generate a secret; use the Base64‑encoded \"name:secret\" as the value for the\n    Authorization header with the \"Basic\" scheme.\n- type: jwt\n  name: Webhook JWT Signature\n  evidence: Avo will sign each webhook call it sends to your endpoint by including a\
  \ JWT token in each request authorization header.\n  location: header\n  header: authorization\n  how_to_obtain: Retrieve the unique secret key for the webhook from the Webhook publishing page in Avo; the JWT token is sent in the Authorization\n    header as a Bearer token.\ndocs: https://www.avo.app/docs/workspace-management/authentication\n"
source_yaml_url: https://artifacts.apis.io/avo-app/authentication/avo-app-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Data Governance
- Analytics
- AI
- SaaS
---
