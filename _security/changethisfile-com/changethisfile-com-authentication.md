---
anonymous_access: false
api_key_in: []
api_specs:
- filename: changethisfile-com-account-api-openapi.yml
  format: yaml
  label: ChangeThisFile Account API
  slug: changethisfile-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/changethisfile-com/openapi/changethisfile-com-account-api-openapi.yml
- filename: changethisfile-com-billing-api-openapi.yml
  format: yaml
  label: ChangeThisFile Billing API
  slug: changethisfile-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/changethisfile-com/openapi/changethisfile-com-billing-api-openapi.yml
- filename: changethisfile-com-conversions-api-openapi.yml
  format: yaml
  label: ChangeThisFile Conversions API
  slug: changethisfile-com-conversions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/changethisfile-com/openapi/changethisfile-com-conversions-api-openapi.yml
- filename: changethisfile-com-jobs-api-openapi.yml
  format: yaml
  label: ChangeThisFile Jobs API
  slug: changethisfile-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/changethisfile-com/openapi/changethisfile-com-jobs-api-openapi.yml
auth_types: []
description: 'The ChangeThisFile API uses bearer tokens. Every request to /v1/* (except POST /v1/keys/free) must include an Authorization header: Authorization: Bearer ctf_sk_...your_key_here...'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: ChangeThisFile Authentication
name_suffix: Authentication
oauth_flows: []
overview: ChangeThisFile declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ChangeThisFile
provider_slug: changethisfile-com
scheme_count: 1
schemes:
- evidence: 'The ChangeThisFile API uses bearer tokens . Every request to /v1/* (except POST /v1/keys/free ) must include an Authorization header: Authorization: Bearer ctf_sk_...your_key_here...'
  header: Authorization
  how_to_obtain: Obtain a secret key (ctf_sk_…) by requesting a free key via POST https://changethisfile.com/v1/keys/free and completing email verification.
  location: header
  name: Bearer
  type: http-bearer
slug: changethisfile-com-authentication
source_filename: changethisfile-com-authentication.yml
source_heading: Authentication Profile
source_url: https://changethisfile.com/docs/authentication
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://changethisfile.com/docs/authentication\nsources:\n- https://changethisfile.com/docs/authentication\n- https://changethisfile.com/docs/quickstart\ndescription: 'The ChangeThisFile API uses bearer tokens. Every request to /v1/* (except POST /v1/keys/free) must include an Authorization header:\n  Authorization: Bearer ctf_sk_...your_key_here...'\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'The ChangeThisFile API uses bearer tokens . Every request to /v1/* (except POST /v1/keys/free ) must include an Authorization header:\n    Authorization: Bearer ctf_sk_...your_key_here...'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain a secret key (ctf_sk_…) by requesting a free key via POST https://changethisfile.com/v1/keys/free and completing email\n    verification.\nnote: No OAuth2, apiKey, or other authentication schemes are documented.\ndocs:\
  \ https://changethisfile.com/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/changethisfile-com/authentication/changethisfile-com-authentication.yml
summary_line: 1 scheme
tags:
- File Conversion
- Free
- Privacy
- Software-as-a-Service
---
