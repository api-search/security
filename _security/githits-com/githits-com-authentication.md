---
anonymous_access: false
api_key_in: []
api_specs:
- filename: githits-com-openapi-generated.yml
  format: yaml
  label: GitHits API
  slug: githits-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/githits-com/openapi/_ae-authored/githits-com-openapi-generated.yml
auth_types: []
description: Authentication methods published for GitHits.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: GitHits Authentication
name_suffix: Authentication
oauth_flows: []
overview: GitHits declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: GitHits
provider_slug: githits-com
scheme_count: 2
schemes:
- evidence: Browser OAuth is the recommended method for local development.
  how_to_obtain: Run `npx githits@latest login` (or `--no-browser` for headless) which opens the GitHits OAuth page in a browser, signs in, and stores the resulting token in the system keychain.
  name: Browser OAuth
  type: oauth2
- evidence: For CI pipelines, automation scripts, and environments where browser login isn't practical, set the `GITHITS_API_TOKEN` environment variable.
  header: Authorization
  how_to_obtain: Create an API token in your token settings (https://app.githits.com/settings/tokens) and set it in the `GITHITS_API_TOKEN` environment variable or supply it as a Bearer token in the `Authorization` header.
  location: header
  name: API token
  type: http-bearer
slug: githits-com-authentication
source_filename: githits-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.githits.com/authentication.md
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.githits.com/authentication.md\nsources:\n- https://docs.githits.com/authentication.md\n- https://docs.githits.com/api/authentication.md\n- https://docs.githits.com/api/authentication\n- https://docs.githits.com/guides/troubleshooting.md\ndescription: Authentication methods published for GitHits.\nschemes:\n- type: oauth2\n  name: Browser OAuth\n  evidence: Browser OAuth is the recommended method for local development.\n  how_to_obtain: Run `npx githits@latest login` (or `--no-browser` for headless) which opens the GitHits OAuth page in a browser, signs in, and\n    stores the resulting token in the system keychain.\n- type: http-bearer\n  name: API token\n  evidence: For CI pipelines, automation scripts, and environments where browser login isn't practical, set the `GITHITS_API_TOKEN` environment\n    variable.\n  location: header\n  header: Authorization\n  how_to_obtain:\
  \ Create an API token in your token settings (https://app.githits.com/settings/tokens) and set it in the `GITHITS_API_TOKEN` environment\n    variable or supply it as a Bearer token in the `Authorization` header.\ndocs: https://docs.githits.com/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/githits-com/authentication/githits-com-authentication.yml
summary_line: 2 schemes
tags:
- Open Source
- Artificial Intelligence
- Coding Agents
- Indexing
- Platform
---
