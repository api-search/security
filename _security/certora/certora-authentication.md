---
api_key_in:
- environment
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Certora Authentication
name_suffix: Authentication
oauth_flows: []
overview: Certora secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Certora
provider_slug: certora
scheme_count: 1
schemes:
- in: environment
  name: personalAccessKey
  parameter: CERTORAKEY
  source: docs.certora.com/en/latest/docs/user-guide/install.html
  type: apiKey
slug: certora-authentication
source_filename: certora-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.certora.com/en/latest/docs/user-guide/install.html\ndocs: https://docs.certora.com/en/latest/docs/user-guide/install.html\nsummary:\n  types: [apiKey]\n  api_key_in: [environment]\nnotes: >-\n  The Certora Prover cloud service is authenticated with a per-user personal\n  access key. After installing certora-cli, the key is obtained from the Certora\n  Prover web application and supplied to the certoraRun tool via the CERTORAKEY\n  environment variable. There is no public OAuth or REST securityScheme; the CLI\n  is the sole documented client of the verification backend.\nschemes:\n- name: personalAccessKey\n  type: apiKey\n  in: environment\n  parameter: CERTORAKEY\n  source: docs.certora.com/en/latest/docs/user-guide/install.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/certora/refs/heads/main/authentication/certora-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Security
- Formal Verification
- Smart Contracts
- Blockchain
- Developer Tools
- CLI
- Web3
---
