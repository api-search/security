---
anonymous_access: false
api_key_in: []
api_specs:
- filename: parseable-api-openapi-generated.yml
  format: yaml
  label: Parseable API Reference API
  slug: api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parseable/openapi/_ae-authored/parseable-api-openapi-generated.yml
- filename: parseable-core-openapi-generated.yml
  format: yaml
  label: Parseable core API
  slug: core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parseable/openapi/_ae-authored/parseable-core-openapi-generated.yml
- filename: parseable-ingest-data-openapi-generated.yml
  format: yaml
  label: Parseable ingest data API
  slug: ingest-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parseable/openapi/_ae-authored/parseable-ingest-data-openapi-generated.yml
- filename: parseable-user-guide-openapi-generated.yml
  format: yaml
  label: Parseable user guide API
  slug: user-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parseable/openapi/_ae-authored/parseable-user-guide-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Parseable Authentication
name_suffix: Authentication
oauth_flows: []
overview: Parseable declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Parseable
provider_slug: parseable
scheme_count: 2
schemes:
- evidence: Send the secret value in the X-API-Key header.
  header: X-API-Key
  how_to_obtain: Create an API key via the Parseable UI or REST API; the full key value is returned only on creation.
  location: header
  name: X-API-Key
  type: apiKey
- authorize_url: <issuer>/authorize
  evidence: OpenID Connect (OIDC) lets Parseable delegate user sign‑in to an identity provider while keeping Parseable roles and permissions in control of what each user can access after login.
  how_to_obtain: Configure OIDC client ID, client secret, and issuer URL in Parseable environment variables; the provider’s discovery URL supplies the actual endpoints.
  name: OpenID Connect
  scopes:
  - openid
  - profile
  - email
  - offline_access
  - groups
  token_url: <issuer>/oauth/token
  type: oauth2
slug: parseable-authentication
source_filename: parseable-authentication.yml
source_heading: Authentication Profile
source_url: https://www.parseable.com/docs/user-guide/api-keys
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.parseable.com/docs/user-guide/api-keys\nsources:\n- https://www.parseable.com/docs/user-guide/api-keys\n- https://www.parseable.com/docs/user-guide/openid\n- https://www.parseable.com/docs/integrations/auth/auth0\n- https://www.parseable.com/docs/integrations/auth/authentik\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: Send the secret value in the X-API-Key header.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create an API key via the Parseable UI or REST API; the full key value is returned only on creation.\n- type: oauth2\n  name: OpenID Connect\n  evidence: OpenID Connect (OIDC) lets Parseable delegate user sign‑in to an identity provider while keeping Parseable roles and permissions in\n    control of what each user can access after login.\n  token_url: <issuer>/oauth/token\n  authorize_url: <issuer>/authorize\n  scopes:\n  - openid\n  -\
  \ profile\n  - email\n  - offline_access\n  - groups\n  how_to_obtain: Configure OIDC client ID, client secret, and issuer URL in Parseable environment variables; the provider’s discovery URL supplies\n    the actual endpoints.\ndocs: https://www.parseable.com/docs/user-guide/api-keys\n"
source_yaml_url: https://artifacts.apis.io/parseable/authentication/parseable-authentication.yml
summary_line: 2 schemes
tags:
- Observability
- OpenTelemetry
- Rust
- Cloud
- Data Lake
- Company
---
