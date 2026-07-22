---
api_key_in:
- header
auth_types:
- apiKey
- awsSignatureV4
description: ''
kind: authentication
layout: security
method: searched
name: Tigris Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tigris secures its APIs with apiKey and awsSignatureV4 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tigris
provider_slug: tigris
scheme_count: 1
schemes:
- description: S3-style access key ID and secret access key. Credentials are generated in the Tigris console (https://console.storage.dev) and passed via the standard AWS environment variables (AWS_ACCESS_KEY_ID / AWS_SECRET_ACCESS_KEY) or SDK credential providers. Requests are signed with AWS Signature Version 4 against the endpoint https://t3.storage.dev (region "auto").
  in: header
  name: AWSAccessKey
  scheme: aws-sigv4
  sources:
  - https://www.tigrisdata.com/docs/sdks/tigris/
  - https://www.tigrisdata.com/llms.txt
  type: apiKey
slug: tigris-authentication
source_filename: tigris-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.tigrisdata.com/docs/iam/ + https://www.tigrisdata.com/docs/sdks/tigris/ + https://console.storage.dev\ndocs: https://www.tigrisdata.com/docs/iam/\nsummary:\n  types: [apiKey, awsSignatureV4]\n  api_key_in: [header]\n  model: S3 access key / secret access key signed with AWS Signature Version 4\nschemes:\n- name: AWSAccessKey\n  type: apiKey\n  description: >-\n    S3-style access key ID and secret access key. Credentials are generated in\n    the Tigris console (https://console.storage.dev) and passed via the standard\n    AWS environment variables (AWS_ACCESS_KEY_ID / AWS_SECRET_ACCESS_KEY) or SDK\n    credential providers. Requests are signed with AWS Signature Version 4\n    against the endpoint https://t3.storage.dev (region \"auto\").\n  in: header\n  scheme: aws-sigv4\n  sources: [https://www.tigrisdata.com/docs/sdks/tigris/, https://www.tigrisdata.com/llms.txt]\naccess_control:\n  model: IAM\n  docs: https://www.tigrisdata.com/docs/iam/\n\
  \  description: >-\n    Tigris provides IAM with users, roles, and bucket policies. Access keys can\n    be scoped to roles (e.g. Editor, ReadOnly) and to specific buckets, including\n    per-fork scoped credentials created by the agent-kit.\n  roles_observed: [Editor]\nnotes:\n- For MCP clients, Tigris publishes mcp-oidc-provider, a vendor-neutral OIDC layer between MCP clients and an upstream IdP (Auth0/Clerk/Okta).\n- No OAuth2 authorization-code flow is used for the core storage (S3) API; it is access-key based, so no scopes/ artifact applies.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tigris/refs/heads/main/authentication/tigris-authentication.yml
summary_line: apiKey/awsSignatureV4 · 1 scheme
tags:
- Company
- Object Storage
- Cloud Storage
- S3 Compatible
- Storage
- AI Infrastructure
- Agents
- Data Infrastructure
---
