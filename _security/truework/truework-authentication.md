---
api_key_in: []
api_specs:
- filename: truework-verifications-orders-openapi.yml
  format: yaml
  label: Truework Verifications API
  slug: truework-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truework/refs/heads/main/openapi/truework-verifications-orders-openapi.yml
- filename: truework-beta-openapi.yml
  format: yaml
  label: Truework Qualifications API (Beta)
  slug: truework-qualifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truework/refs/heads/main/openapi/truework-beta-openapi.yml
- filename: truework-beta-openapi.yml
  format: yaml
  label: Truework Tenant Properties API (Beta)
  slug: truework-tenant-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truework/refs/heads/main/openapi/truework-beta-openapi.yml
- filename: truework-webhooks-openapi.yml
  format: yaml
  label: Truework Webhooks
  slug: truework-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truework/refs/heads/main/openapi/truework-webhooks-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Truework Authentication
name_suffix: Authentication
oauth_flows: []
overview: Truework secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Truework
provider_slug: truework
scheme_count: 1
schemes:
- description: 'Bearer tokens conform to the [RFC6750](https://datatracker.ietf.org/doc/html/rfc6750#section-2.1) spec.



    Production API keys (secret keys) are prefixed with `tw_sk_` and sandbox keys are prefixed with `tw_sk_test_`. If your secret key is published, you should rotate your API keys.


    Truework.JS publishable keys are prefixed with `tw_pk_` and `tw_pk_test` respectively.



    **Examples**

    - For Authoriz'
  name: Bearer
  scheme: bearer
  sources:
  - openapi/truework-beta-openapi.yml
  - openapi/truework-verifications-orders-openapi.yml
  type: http
slug: truework-authentication
source_filename: truework-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/truework-beta-openapi.yml, openapi/truework-verifications-orders-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  description: |-\n    Bearer tokens conform to the [RFC6750](https://datatracker.ietf.org/doc/html/rfc6750#section-2.1) spec.\n\n\n    Production API keys (secret keys) are prefixed with `tw_sk_` and sandbox keys are prefixed with `tw_sk_test_`. If your secret key is published, you should rotate your API keys.\n\n    Truework.JS publishable keys are prefixed with `tw_pk_` and `tw_pk_test` respectively.\n\n\n    **Examples**\n    - For Authoriz\n  sources:\n  - openapi/truework-beta-openapi.yml\n  - openapi/truework-verifications-orders-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truework/refs/heads/main/authentication/truework-authentication.yml
summary_line: http · 1 scheme
tags:
- Verifications
- Income Verification
- Employment Verification
- VOIE
- Mortgage
- Lending
- Credit Unions
- Identity
- KYC
- Fintech
---
