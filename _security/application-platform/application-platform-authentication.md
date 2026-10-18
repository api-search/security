---
anonymous_access: false
api_key_in: []
api_specs:
- filename: application-platform-doppelt-digital-api-api-openapi.yml
  format: yaml
  label: doppelt.digital Doppelt.digital API
  slug: application-platform-doppelt-digital-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/application-platform/refs/heads/main/openapi/application-platform-doppelt-digital-api-api-openapi.yml
- filename: application-platform-install-api-openapi.yml
  format: yaml
  label: doppelt.digital Install API
  slug: application-platform-install-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/application-platform/refs/heads/main/openapi/application-platform-install-api-openapi.yml
auth_types: []
description: Authentication schemes described in the provided pages for MainPath and its connections.
kind: authentication
layout: security
mechanism_count: 6
method: searched
name: Application Platform Authentication
name_suffix: Authentication
oauth_flows: []
overview: doppelt.digital declares 6 security scheme(s) across its OpenAPI definitions.
provider_name: doppelt.digital
provider_slug: application-platform
scheme_count: 6
schemes:
- evidence: Personal API keys let the mp CLI, your CI runs and your own scripts authenticate against MainPath without anyone signing in through a browser.
  how_to_obtain: Create a personal API key in your account settings; the secret value is shown once after creation.
  name: Personal API Key
  type: apiKey
- evidence: If OAuth is unavailable, store a personal access token.
  how_to_obtain: Create a token in GitHub under Settings → Developer settings → Personal access tokens with repository, workflow, and package access.
  name: GitHub Personal Access Token
  type: apiKey
- evidence: Connect with GitHub (OAuth) is the recommended path.
  how_to_obtain: Configure a GitHub OAuth app for MainPath (client ID and secret) and use the Connections UI to authorize.
  name: GitHub OAuth
  type: oauth2
- evidence: Otherwise store a personal access token; that also covers self‑hosted instances.
  how_to_obtain: Create a token in GitLab under Preferences → Access Tokens (or Group → Access Tokens) with the api scope.
  name: GitLab Personal Access Token
  type: apiKey
- evidence: Connect with GitLab (OAuth against GitLab.com) is recommended.
  how_to_obtain: Configure a GitLab OAuth app for MainPath (client ID and secret) and use the Connections UI to authorize.
  name: GitLab OAuth
  type: oauth2
- evidence: The official third‑party path is an API key from the OpenAI Platform.
  how_to_obtain: Create a key in the OpenAI Platform under API keys and store it in MainPath Connections.
  name: OpenAI API Key
  type: apiKey
slug: application-platform-authentication
source_filename: application-platform-authentication.yml
source_heading: Authentication Profile
source_url: https://www.mainpath.ai/en/blog/api-keys/index.md
source_yaml: "generated: '2026-10-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.mainpath.ai/en/blog/api-keys/index.md\nsources:\n- https://www.mainpath.ai/en/blog/api-keys/index.md\n- https://www.mainpath.ai/en/docs/github-credentials/index.md\n- https://www.mainpath.ai/en/docs/gitlab-credentials/index.md\n- https://www.mainpath.ai/en/docs/openai-credentials/index.md\ndescription: Authentication schemes described in the provided pages for MainPath and its connections.\nschemes:\n- type: apiKey\n  name: Personal API Key\n  evidence: Personal API keys let the mp CLI, your CI runs and your own scripts authenticate against MainPath without anyone signing in through\n    a browser.\n  how_to_obtain: Create a personal API key in your account settings; the secret value is shown once after creation.\n- type: apiKey\n  name: GitHub Personal Access Token\n  evidence: If OAuth is unavailable, store a personal access token.\n  how_to_obtain: Create a token\
  \ in GitHub under Settings → Developer settings → Personal access tokens with repository, workflow, and package\n    access.\n- type: oauth2\n  name: GitHub OAuth\n  evidence: Connect with GitHub (OAuth) is the recommended path.\n  how_to_obtain: Configure a GitHub OAuth app for MainPath (client ID and secret) and use the Connections UI to authorize.\n- type: apiKey\n  name: GitLab Personal Access Token\n  evidence: Otherwise store a personal access token; that also covers self‑hosted instances.\n  how_to_obtain: Create a token in GitLab under Preferences → Access Tokens (or Group → Access Tokens) with the api scope.\n- type: oauth2\n  name: GitLab OAuth\n  evidence: Connect with GitLab (OAuth against GitLab.com) is recommended.\n  how_to_obtain: Configure a GitLab OAuth app for MainPath (client ID and secret) and use the Connections UI to authorize.\n- type: apiKey\n  name: OpenAI API Key\n  evidence: The official third‑party path is an API key from the OpenAI Platform.\n  how_to_obtain:\
  \ Create a key in the OpenAI Platform under API keys and store it in MainPath Connections.\ndocs: https://www.mainpath.ai/en/blog/api-keys/index.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/application-platform/refs/heads/main/authentication/application-platform-authentication.yml
summary_line: 6 schemes
tags:
- Low-code
- Development Platform
- Cloud Hosting
- European SaaS
- Automation
---
