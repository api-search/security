---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gitkraken-openapi-generated.yml
  format: yaml
  label: GitKraken API
  slug: gitkraken-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitkraken/refs/heads/main/openapi/_ae-authored/gitkraken-openapi-generated.yml
auth_types: []
description: Authentication methods for GitKraken Desktop when accessing Git hosts without a dedicated integration page.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Gitkraken Authentication
name_suffix: Authentication
oauth_flows: []
overview: GitKraken declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: GitKraken
provider_slug: gitkraken
scheme_count: 2
schemes:
- evidence: How HTTPS authentication works – This is the default and most common method for interacting with remotes. It requires your Git username and password.
  header: Authorization
  how_to_obtain: Enter your Git host username and password (or personal access token) when prompted during clone or push.
  location: header
  name: HTTPS Basic Authentication
  type: http-basic
- evidence: How SSH authentication works – Before cloning via SSH, you must first set up your SSH keys in GitKraken Desktop.
  how_to_obtain: Generate a new SSH key pair or browse to an existing one in Preferences > SSH, then add the public key to the hosting service.
  location: ssh
  name: SSH Key Authentication
  type: other
slug: gitkraken-authentication
source_filename: gitkraken-authentication.yml
source_heading: Authentication Profile
source_url: https://help.gitkraken.com/gitkraken-desktop/authentication/
source_yaml: "generated: '2026-09-22'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://help.gitkraken.com/gitkraken-desktop/authentication/\nsources:\n- https://help.gitkraken.com/gitkraken-desktop/authentication/\n- https://help.gitkraken.com/gitkraken-desktop/commit-signing-with-gpg/\n- https://help.gitkraken.com/gitkraken-desktop/how-to-install/\n- https://help.gitkraken.com/gitkraken-desktop/serverless/\ndescription: Authentication methods for GitKraken Desktop when accessing Git hosts without a dedicated integration page.\nschemes:\n- type: http-basic\n  name: HTTPS Basic Authentication\n  evidence: How HTTPS authentication works – This is the default and most common method for interacting with remotes. It requires your Git username\n    and password.\n  location: header\n  header: Authorization\n  how_to_obtain: Enter your Git host username and password (or personal access token) when prompted during clone or push.\n- type: other\n  name: SSH Key Authentication\n\
  \  evidence: How SSH authentication works – Before cloning via SSH, you must first set up your SSH keys in GitKraken Desktop.\n  location: ssh\n  how_to_obtain: Generate a new SSH key pair or browse to an existing one in Preferences > SSH, then add the public key to the hosting service.\ndocs: https://help.gitkraken.com/gitkraken-desktop/authentication/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gitkraken/refs/heads/main/authentication/gitkraken-authentication.yml
summary_line: 2 schemes
tags:
- Developer Tools
- Git
- Artificial Intelligence
- Collaboration
- Platform
---
