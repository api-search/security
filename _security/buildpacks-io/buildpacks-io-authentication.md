---
anonymous_access: false
api_key_in: []
api_specs:
- filename: buildpacks-io-buildpacks-api-openapi.yml
  format: yaml
  label: buildpacks-io Buildpacks API
  slug: buildpacks-io-buildpacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildpacks-io/refs/heads/main/openapi/buildpacks-io-buildpacks-api-openapi.yml
- filename: buildpacks-io-search-api-openapi.yml
  format: yaml
  label: buildpacks-io Search API
  slug: buildpacks-io-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildpacks-io/refs/heads/main/openapi/buildpacks-io-search-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Buildpacks Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Buildpacks Io declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Buildpacks Io
provider_slug: buildpacks-io
scheme_count: 0
schemes: []
slug: buildpacks-io-authentication
source_filename: buildpacks-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: >-\n  Live unauthenticated probes of registry.buildpacks.io/api/v1, the registry-api README\n  (https://github.com/buildpacks/registry-api) and the Buildpack Registry Extension Specification\n  (https://github.com/buildpacks/spec/blob/main/extensions/buildpack-registry.md)\ndocs: https://github.com/buildpacks/spec/blob/main/extensions/buildpack-registry.md\nsummary: >-\n  The public buildpack registry API is read-only and entirely unauthenticated — no key, token,\n  account or signup. All three operations return 200 to an anonymous request. Write access to the\n  registry is not an API surface at all: publishing and yanking go through the `pack` CLI, which\n  opens a GitHub issue against buildpacks/registry-index and authenticates with a GitHub token\n  belonging to the buildpack author, not with a registry credential.\nschemes: []\nauth_required: false\nanonymous_access: full\nevidence:\n- url: https://registry.buildpacks.io/api/v1/search?matches=ruby\n\
  \  status: 200\n  note: no Authorization header sent\n- url: https://registry.buildpacks.io/api/v1/buildpacks/paketo-buildpacks/nodejs/10.11.0\n  status: 200\n  note: no Authorization header sent\n- url: https://registry.buildpacks.io/.well-known/oauth-authorization-server\n  status: 404\n- url: https://registry.buildpacks.io/.well-known/openid-configuration\n  status: 404\nwrite_path:\n  mechanism: GitHub issue against buildpacks/registry-index, opened by `pack buildpack register`\n  credential: the author's GitHub token\n  not_an_api: true\n  source: https://github.com/buildpacks/spec/blob/main/extensions/buildpack-registry.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buildpacks-io/refs/heads/main/authentication/buildpacks-io-authentication.yml
summary_line: 0 schemes
tags:
- Cloud Native Buildpacks
- Container Images
- Build Automation
- CNCF
- Open-Source
- Developer Tools
- OCI
- Specification
- Supply Chain
- Registry
---
