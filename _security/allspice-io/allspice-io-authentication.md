---
anonymous_access: false
api_key_in: []
api_specs:
- filename: allspice-io-repos-api-openapi.yml
  format: yaml
  label: AllSpice.io Repos API
  slug: allspice-io-repos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allspice-io/refs/heads/main/openapi/allspice-io-repos-api-openapi.yml
auth_types: []
description: Authentication methods for AllSpice Git operations
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Allspice Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: AllSpice.io declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AllSpice.io
provider_slug: allspice-io
scheme_count: 1
schemes:
- evidence: Authentication is handled via OAuth HTTPS using your web browser.
  how_to_obtain: When pushing or pulling, the Git client opens a browser to log in to hub.allspice.io and grant permissions.
  name: OAuth HTTPS
  type: oauth2
slug: allspice-io-authentication
source_filename: allspice-io-authentication.yml
source_heading: Authentication Profile
source_url: https://learn.allspice.io/docs/authentication-setup.md
source_yaml: "generated: '2026-10-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://learn.allspice.io/docs/authentication-setup.md\nsources:\n- https://learn.allspice.io/docs/authentication-setup.md\n- https://learn.allspice.io/docs/how-to-create-an-allspice-authentication-application-access-token.md\n- https://learn.allspice.io/docs/github-desktop-ssh.md\n- https://learn.allspice.io/docs/setting-up-openssh-authentication-with-git.md\ndescription: Authentication methods for AllSpice Git operations\nschemes:\n- type: oauth2\n  name: OAuth HTTPS\n  evidence: Authentication is handled via OAuth HTTPS using your web browser.\n  how_to_obtain: When pushing or pulling, the Git client opens a browser to log in to hub.allspice.io and grant permissions.\ndocs: https://learn.allspice.io/docs/authentication-setup.md\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allspice-io/refs/heads/main/authentication/allspice-io-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Hardware
- Collaboration
- Artificial Intelligence
- Design
---
