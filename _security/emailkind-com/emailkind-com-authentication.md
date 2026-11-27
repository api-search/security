---
anonymous_access: false
api_key_in: []
api_specs:
- filename: emailkind-com-classify-api-openapi.yml
  format: yaml
  label: EmailKind Classify API
  slug: emailkind-com-classify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emailkind-com/openapi/emailkind-com-classify-api-openapi.yml
- filename: emailkind-com-signup-api-openapi.yml
  format: yaml
  label: EmailKind Signup API
  slug: emailkind-com-signup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emailkind-com/openapi/emailkind-com-signup-api-openapi.yml
auth_types: []
description: Authentication schemes for EmailKind API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: EmailKind Authentication
name_suffix: Authentication
oauth_flows: []
overview: EmailKind declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: EmailKind
provider_slug: emailkind-com
scheme_count: 1
schemes:
- evidence: All API requests require authentication via an API key passed in the Authorization header.
  header: Authorization
  how_to_obtain: Obtain via dashboard or programmatically through the two‑step signup flow described on the Getting Started pages.
  location: header
  name: API Key
  type: apiKey
slug: emailkind-com-authentication
source_filename: emailkind-com-authentication.yml
source_heading: Authentication Profile
source_url: https://emailkind.com/docs/authentication
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://emailkind.com/docs/authentication\nsources:\n- https://emailkind.com/docs/authentication\n- https://emailkind.com/fr/docs/authentication\n- https://emailkind.com/docs/getting-started\n- https://emailkind.com/fr/docs/getting-started\ndescription: Authentication schemes for EmailKind API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: All API requests require authentication via an API key passed in the Authorization header.\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain via dashboard or programmatically through the two‑step signup flow described on the Getting Started pages.\nnote: No OAuth2, http-bearer, http-basic, jwt, hmac, mtls, or other schemes are documented.\ndocs: https://emailkind.com/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/emailkind-com/authentication/emailkind-com-authentication.yml
summary_line: 1 scheme
tags:
- Email
- Email Verification
- Data Enrichment
- Software-as-a-Service
---
