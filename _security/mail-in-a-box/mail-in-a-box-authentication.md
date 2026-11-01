---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mail-in-a-box-dns-api-openapi.yml
  format: yaml
  label: Mail-in-a-Box DNS API
  slug: mail-in-a-box-dns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mail-in-a-box/openapi/mail-in-a-box-dns-api-openapi.yml
- filename: mail-in-a-box-mail-api-openapi.yml
  format: yaml
  label: Mail-in-a-Box Mail API
  slug: mail-in-a-box-mail-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mail-in-a-box/openapi/mail-in-a-box-mail-api-openapi.yml
- filename: mail-in-a-box-mfa-api-openapi.yml
  format: yaml
  label: Mail-in-a-Box MFA API
  slug: mail-in-a-box-mfa-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mail-in-a-box/openapi/mail-in-a-box-mfa-api-openapi.yml
- filename: mail-in-a-box-ssl-api-openapi.yml
  format: yaml
  label: Mail-in-a-Box SSL API
  slug: mail-in-a-box-ssl-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mail-in-a-box/openapi/mail-in-a-box-ssl-api-openapi.yml
- filename: mail-in-a-box-system-api-openapi.yml
  format: yaml
  label: Mail-in-a-Box System API
  slug: mail-in-a-box-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mail-in-a-box/openapi/mail-in-a-box-system-api-openapi.yml
- filename: mail-in-a-box-user-api-openapi.yml
  format: yaml
  label: Mail-in-a-Box User API
  slug: mail-in-a-box-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mail-in-a-box/openapi/mail-in-a-box-user-api-openapi.yml
- filename: mail-in-a-box-web-api-openapi.yml
  format: yaml
  label: Mail-in-a-Box Web API
  slug: mail-in-a-box-web-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mail-in-a-box/openapi/mail-in-a-box-web-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Mail In A Box Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mail-in-a-Box secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mail-in-a-Box
provider_slug: mail-in-a-box
scheme_count: 1
schemes:
- description: 'Credentials can be supplied using the `Authorization` header in

    format `Authorization: Basic {access-token}`.


    The `access-token` is comprised of the Base64 encoding of `username:password`.

    The `username` is the mail user''s email address, and `password` can either be the mail user''s

    password, or the `api_key` returned from the `login` operation.


    When using `curl`, you can supply user credentials '
  name: basicAuth
  scheme: basic
  sources:
  - openapi/mailinabox-openapi.yml
  type: http
slug: mail-in-a-box-authentication
source_filename: mail-in-a-box-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: derived\nsource: openapi/mailinabox-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: \"Credentials can be supplied using the `Authorization` header in\\nformat `Authorization:\\\n    \\ Basic {access-token}`.\\n\\nThe `access-token` is comprised of the Base64 encoding of `username:password`.\\n\\\n    The `username` is the mail user's email address, and `password` can either be the mail user's\\n\\\n    password, or the `api_key` returned from the `login` operation.\\n\\nWhen using `curl`, you\\\n    \\ can supply user credentials \"\n  sources:\n  - openapi/mailinabox-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/mail-in-a-box/authentication/mail-in-a-box-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Email
- Self-hosted
- Open-source
- Automation
- Privacy
---
