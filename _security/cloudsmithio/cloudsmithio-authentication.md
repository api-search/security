---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cloudsmithio-metadata-api-openapi.yml
  format: yaml
  label: Cloudsmithio Metadata API
  slug: cloudsmithio-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudsmithio/refs/heads/main/openapi/cloudsmithio-metadata-api-openapi.yml
- filename: cloudsmithio-package-api-openapi.yml
  format: yaml
  label: Cloudsmithio Package API
  slug: cloudsmithio-package-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudsmithio/refs/heads/main/openapi/cloudsmithio-package-api-openapi.yml
- filename: cloudsmithio-user-api-openapi.yml
  format: yaml
  label: Cloudsmithio User API
  slug: cloudsmithio-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudsmithio/refs/heads/main/openapi/cloudsmithio-user-api-openapi.yml
auth_types: []
description: Authentication methods supported by Cloudsmith as described in the documentation.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Cloudsmithio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cloudsmithio declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Cloudsmithio
provider_slug: cloudsmithio
scheme_count: 1
schemes:
- evidence: 'Cloudsmith supports the following authentication methods: Single sign-on via Security Assertion Markup Language (SAML)'
  name: SAML
  type: other
slug: cloudsmithio-authentication
source_filename: cloudsmithio-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.cloudsmith.com/authentication
source_yaml: "generated: '2026-10-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.cloudsmith.com/authentication\nsources:\n- https://docs.cloudsmith.com/authentication\n- https://docs.cloudsmith.com/authentication/single-sign-on\n- https://docs.cloudsmith.com/authentication/single-sign-on-with-entra-id\n- https://docs.cloudsmith.com/authentication/single-sign-on-with-google-g-suite\ndescription: Authentication methods supported by Cloudsmith as described in the documentation.\nschemes:\n- type: other\n  name: SAML\n  evidence: 'Cloudsmith supports the following authentication methods: Single sign-on via Security Assertion Markup Language (SAML)'\ndocs: https://docs.cloudsmith.com/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudsmithio/refs/heads/main/authentication/cloudsmithio-authentication.yml
summary_line: 1 scheme
tags:
- Artifact Management
- Software Supply Chain
- Security
- DevOps
- Cloud
---
