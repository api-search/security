---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bitbank-openapi-generated.yml
  format: yaml
  label: bitbank API
  slug: bitbank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitbank/refs/heads/main/openapi/_ae-authored/bitbank-openapi-generated.yml
auth_types: []
description: Authentication methods for GitHub via SSH as described in the provided documentation.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Bitbank Authentication
name_suffix: Authentication
oauth_flows: []
overview: bitbank declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: bitbank
provider_slug: bitbank
scheme_count: 1
schemes:
- evidence: When you connect via SSH, you authenticate using a private key file on your local machine.
  how_to_obtain: Add the public key to your GitHub account.
  location: ssh
  name: SSH
  type: other
slug: bitbank-authentication
source_filename: bitbank-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.github.com/en/authentication/connecting-to-github-with-ssh
source_yaml: "generated: '2026-09-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.github.com/en/authentication/connecting-to-github-with-ssh\nsources:\n- https://docs.github.com/en/authentication/connecting-to-github-with-ssh\n- https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account\n- https://docs.github.com/en/authentication/connecting-to-github-with-ssh/checking-for-existing-ssh-keys\n- https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent\ndescription: Authentication methods for GitHub via SSH as described in the provided documentation.\nschemes:\n- type: other\n  name: SSH\n  evidence: When you connect via SSH, you authenticate using a private key file on your local machine.\n  location: ssh\n  how_to_obtain: Add the public key to your GitHub account.\ndocs: https://docs.github.com/en/authentication/connecting-to-github-with-ssh\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitbank/refs/heads/main/authentication/bitbank-authentication.yml
summary_line: 1 scheme
tags:
- Cryptocurrency
- Exchange
- Japan
- API
- Finance
---
