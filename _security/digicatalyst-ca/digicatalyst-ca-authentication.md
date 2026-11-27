---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: DigiCatalyst Systems Authentication
name_suffix: Authentication
oauth_flows: []
overview: DigiCatalyst Systems declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: DigiCatalyst Systems
provider_slug: digicatalyst-ca
scheme_count: 2
schemes:
- applies_to: hosted MCP endpoint https://dep-diff.digicatalyst.ca/mcp
  description: The README documents no credential for the hosted endpoint; "The hosted instance authenticates to GitHub with its own token". A caller may optionally pass ?githubToken=ghp_xxx on the URL so GitHub requests count against their own GitHub rate limit.
  name: none
  type: none
- applies_to: local stdio server (npx @digicatalyst/dep-diff-mcp)
  description: Optional third-party GitHub token (env GITHUB_TOKEN, or the gh CLI's `gh auth token`) used only to read GitHub release notes; it is not a DigiCatalyst credential. README recommends least-privilege, public-repo-read-only tokens.
  in: env
  name: GITHUB_TOKEN
  type: apiKey
slug: digicatalyst-ca-authentication
source_filename: digicatalyst-ca-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://github.com/DigiCatalyst-Systems/dep-diff-mcp#hosted-remote-no-install\ndocs: https://github.com/DigiCatalyst-Systems/dep-diff-mcp#github-token-optional-but-recommended\nschemes:\n- name: none\n  type: none\n  applies_to: hosted MCP endpoint https://dep-diff.digicatalyst.ca/mcp\n  description: The README documents no credential for the hosted endpoint; \"The hosted instance authenticates to GitHub with its own token\". A caller may optionally pass ?githubToken=ghp_xxx on the URL so GitHub requests count against their own GitHub rate limit.\n- name: GITHUB_TOKEN\n  type: apiKey\n  in: env\n  applies_to: local stdio server (npx @digicatalyst/dep-diff-mcp)\n  description: Optional third-party GitHub token (env GITHUB_TOKEN, or the gh CLI's `gh auth token`) used only to read GitHub release notes; it is not a DigiCatalyst credential. README recommends least-privilege, public-repo-read-only tokens.\nnote: No public HTTP API\
  \ is documented. The company's only documented programmatic surface is the dep-diff MCP server; it has no DigiCatalyst-issued keys, OAuth or scopes.\n"
source_yaml_url: https://artifacts.apis.io/digicatalyst-ca/authentication/digicatalyst-ca-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Web Design
- SEO
- Local SEO
- Automation
- Small Business
- Canada
- Toronto
---
