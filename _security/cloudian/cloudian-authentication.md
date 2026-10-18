---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication for the API is typically handled using AWS Signature Version 4 to ensure secure access and integrity of the requests.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Cloudian Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cloudian declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Cloudian
provider_slug: cloudian
scheme_count: 1
schemes:
- evidence: Authentication for the API is typically handled using AWS Signature Version 4 to ensure secure access and integrity of the requests.
  header: Authorization
  location: header
  name: AWS Signature Version 4
  type: other
slug: cloudian-authentication
source_filename: cloudian-authentication.yml
source_heading: Authentication Profile
source_url: https://cloudian.com/blog/s3-api-actions-authentication-and-code-examples/
source_yaml: "generated: '2026-10-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://cloudian.com/blog/s3-api-actions-authentication-and-code-examples/\nsources:\n- https://cloudian.com/blog/s3-api-actions-authentication-and-code-examples/\ndescription: Authentication for the API is typically handled using AWS Signature Version 4 to ensure secure access and integrity of the requests.\nschemes:\n- type: other\n  name: AWS Signature Version 4\n  evidence: Authentication for the API is typically handled using AWS Signature Version 4 to ensure secure access and integrity of the requests.\n  location: header\n  header: Authorization\ndocs: https://cloudian.com/blog/s3-api-actions-authentication-and-code-examples/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudian/refs/heads/main/authentication/cloudian-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Storage
- Object-Storage
- Artificial Intelligence
- Enterprise
---
