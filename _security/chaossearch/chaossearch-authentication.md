---
anonymous_access: false
api_key_in: []
api_specs:
- filename: chaossearch-openapi-generated.yml
  format: yaml
  label: ChaosSearch API
  slug: chaossearch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaossearch/refs/heads/main/openapi/_ae-authored/chaossearch-openapi-generated.yml
auth_types: []
description: Authentication schemes for ChaosSearch APIs
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Chaossearch Authentication
name_suffix: Authentication
oauth_flows: []
overview: ChaosSearch declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ChaosSearch
provider_slug: chaossearch
scheme_count: 1
schemes:
- evidence: The token can be used as part of a specific `x-amz-security-token` header in REST requests when calling the ChaosSearch APIs.
  header: x-amz-security-token
  how_to_obtain: Obtain a JWT by calling the POST /user/login endpoint with Username, Password (and ParentUid for subaccounts) and then use the returned Token value.
  location: header
  name: JWT token
  type: jwt
slug: chaossearch-authentication
source_filename: chaossearch-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.chaossearch.io/docs/chaossearch-rbac.md
source_yaml: "generated: '2026-10-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.chaossearch.io/docs/chaossearch-rbac.md\nsources:\n- https://docs.chaossearch.io/docs/chaossearch-rbac.md\n- https://docs.chaossearch.io/docs/authentication.md\n- https://docs.chaossearch.io/reference/post_user-login.md\n- https://docs.chaossearch.io/reference/post_user-credential-apikey-create.md\ndescription: Authentication schemes for ChaosSearch APIs\nschemes:\n- type: jwt\n  name: JWT token\n  evidence: The token can be used as part of a specific `x-amz-security-token` header in REST requests when calling the ChaosSearch APIs.\n  location: header\n  header: x-amz-security-token\n  how_to_obtain: Obtain a JWT by calling the POST /user/login endpoint with Username, Password (and ParentUid for subaccounts) and then use the\n    returned Token value.\nnote: Other authentication methods such as AWS SigV4 signing are described but not represented as a standard scheme\
  \ type in this catalog.\ndocs: https://docs.chaossearch.io/docs/chaossearch-rbac.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chaossearch/refs/heads/main/authentication/chaossearch-authentication.yml
summary_line: 1 scheme
tags:
- Analytics
- Observability
- Security
- Data Lake
- Cloud Storage
- ELK
---
