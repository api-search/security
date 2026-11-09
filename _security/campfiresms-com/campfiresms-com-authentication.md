---
anonymous_access: false
api_key_in: []
api_specs:
- filename: campfiresms-com-auth-api-openapi.yml
  format: yaml
  label: Campfire SMS Auth API
  slug: campfiresms-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/campfiresms-com/openapi/campfiresms-com-auth-api-openapi.yml
- filename: campfiresms-com-bridges-api-openapi.yml
  format: yaml
  label: Campfire SMS Bridges API
  slug: campfiresms-com-bridges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/campfiresms-com/openapi/campfiresms-com-bridges-api-openapi.yml
- filename: campfiresms-com-credential-api-openapi.yml
  format: yaml
  label: Campfire SMS Credential API
  slug: campfiresms-com-credential-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/campfiresms-com/openapi/campfiresms-com-credential-api-openapi.yml
- filename: campfiresms-com-enrollment-api-openapi.yml
  format: yaml
  label: Campfire SMS Enrollment API
  slug: campfiresms-com-enrollment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/campfiresms-com/openapi/campfiresms-com-enrollment-api-openapi.yml
- filename: campfiresms-com-health-api-openapi.yml
  format: yaml
  label: Campfire SMS Health API
  slug: campfiresms-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/campfiresms-com/openapi/campfiresms-com-health-api-openapi.yml
- filename: campfiresms-com-installations-api-openapi.yml
  format: yaml
  label: Campfire SMS Installations API
  slug: campfiresms-com-installations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/campfiresms-com/openapi/campfiresms-com-installations-api-openapi.yml
- filename: campfiresms-com-join-api-openapi.yml
  format: yaml
  label: Campfire SMS Join API
  slug: campfiresms-com-join-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/campfiresms-com/openapi/campfiresms-com-join-api-openapi.yml
- filename: campfiresms-com-login-api-openapi.yml
  format: yaml
  label: Campfire SMS Login API
  slug: campfiresms-com-login-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/campfiresms-com/openapi/campfiresms-com-login-api-openapi.yml
- filename: campfiresms-com-public-api-openapi.yml
  format: yaml
  label: Campfire SMS Public API
  slug: campfiresms-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/campfiresms-com/openapi/campfiresms-com-public-api-openapi.yml
- filename: campfiresms-com-setup-api-openapi.yml
  format: yaml
  label: Campfire SMS Setup API
  slug: campfiresms-com-setup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/campfiresms-com/openapi/campfiresms-com-setup-api-openapi.yml
- filename: campfiresms-com-webhooks-api-openapi.yml
  format: yaml
  label: Campfire SMS Webhooks API
  slug: campfiresms-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/campfiresms-com/openapi/campfiresms-com-webhooks-api-openapi.yml
auth_types: []
description: Campfire SMS uses an installation credential as an HTTP Bearer token for MCP and REST requests.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Campfiresms Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Campfire SMS declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Campfire SMS
provider_slug: campfiresms-com
scheme_count: 1
schemes:
- evidence: 'Authenticated MCP and bridge REST requests use the installation credential as an HTTP bearer:


    `Authorization: Bearer <installation-credential>`'
  header: Authorization
  how_to_obtain: Create an installation via the Campfire SMS web UI (Add computers → Create install command) which returns a one‑time installation credential.
  location: header
  name: Installation Credential
  type: http-bearer
slug: campfiresms-com-authentication
source_filename: campfiresms-com-authentication.yml
source_heading: Authentication Profile
source_url: https://campfiresms.com/auth.md
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://campfiresms.com/auth.md\nsources:\n- https://campfiresms.com/auth.md\n- https://campfiresms.com/install.html#local-agents\n- https://campfiresms.com/install.html\ndescription: Campfire SMS uses an installation credential as an HTTP Bearer token for MCP and REST requests.\nschemes:\n- type: http-bearer\n  name: Installation Credential\n  evidence: 'Authenticated MCP and bridge REST requests use the installation credential as an HTTP bearer:\n\n\n    `Authorization: Bearer <installation-credential>`'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an installation via the Campfire SMS web UI (Add computers → Create install command) which returns a one‑time installation\n    credential.\nnote: Campfire SMS does not support OAuth or other authentication schemes.\ndocs: https://campfiresms.com/auth.md\n"
source_yaml_url: https://artifacts.apis.io/campfiresms-com/authentication/campfiresms-com-authentication.yml
summary_line: 1 scheme
tags:
- SMS
- Artificial Intelligence
- Automation
- Messaging
- Integration
---
