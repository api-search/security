---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for BlockchainAnalysis.io API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Blockchainanalysis Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: BlockchainAnalysis.io declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: BlockchainAnalysis.io
provider_slug: blockchainanalysis-io
scheme_count: 1
schemes:
- evidence: 'Every call to the BlockchainAnalysis.io API carries an API key in the Authorization header:'
  header: Authorization
  how_to_obtain: Create a key in the BA | API → Overview & Keys page; the key starts with ba_live_ and is shown only once.
  location: header
  name: Authorization
  type: http-bearer
slug: blockchainanalysis-io-authentication
source_filename: blockchainanalysis-io-authentication.yml
source_heading: Authentication Profile
source_url: https://blockchainanalysis.io/docs/api-reference/authentication
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://blockchainanalysis.io/docs/api-reference/authentication\nsources:\n- https://blockchainanalysis.io/docs/api-reference/authentication\n- https://blockchainanalysis.io/tools/token-security\n- https://blockchainanalysis.io/api/tools/token-security?address=0xdac17f958d2ee523a2206206994597c13d831ec7&chain=ETH\n- https://blockchainanalysis.io/api/tools/approval/scan?address=0x12d66f87a04a9e220743712ce6d9bb1b5616b8fc\ndescription: Authentication schemes for BlockchainAnalysis.io API\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: 'Every call to the BlockchainAnalysis.io API carries an API key in the Authorization header:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in the BA | API → Overview & Keys page; the key starts with ba_live_ and is shown only once.\nnote: No OAuth2, apiKey in query/body, or other authentication methods\
  \ are documented.\ndocs: https://blockchainanalysis.io/docs/api-reference/authentication\n"
source_yaml_url: https://artifacts.apis.io/blockchainanalysis-io/authentication/blockchainanalysis-io-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Compliance
- Blockchain
- AML
- Transaction Monitoring
---
