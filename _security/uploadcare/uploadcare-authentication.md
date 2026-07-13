---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Uploadcare REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://uploadcare.com/api-refs/rest-api/v0.7.0/
- filename: openapi.yaml
  format: yaml
  label: Uploadcare Upload API
  slug: upload-api
  spec_type: OpenAPI
  url: https://uploadcare.com/api-refs/upload-api/
- filename: uploadcare-cdn-api-openapi.yml
  format: yaml
  label: Uploadcare CDN & Image Transformation API
  slug: cdn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uploadcare/refs/heads/main/openapi/uploadcare-cdn-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Uploadcare Authentication
name_suffix: Authentication
oauth_flows: []
overview: Uploadcare secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Uploadcare
provider_slug: uploadcare
scheme_count: 3
schemes:
- description: 'Every request made to `https://api.uploadcare.com/` MUST be signed. HTTPS SHOULD be used with any authorization scheme.


    Requests MUST contain the `Authorization` header defining `auth-scheme` and `auth-param`: `Authorization: auth-scheme auth-param`.


    Every request MUST contain the `Accept` header identifying the REST API version: `Accept: application/vnd.uploadcare-v0.7+json`.


    There are two ava'
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/uploadcare-rest-api-openapi.yml
  type: apiKey
- description: 'With the `Uploadcare` authentication method:

    * `auth-param` is a `public_key:signature` pair, where your `secret_key` is used to derive `signature` but is _not included in every request_ itself.

    * You MUST also provide the `Date` header in [RFC2822](https://datatracker.ietf.org/doc/html/rfc2822#section-3.3) format with the time zone set to `GMT` (see the example below).

    * The date you provide MUST'
  in: header
  name: Uploadcare
  parameter: Uploadcare
  sources:
  - openapi/uploadcare-rest-api-openapi.yml
  type: apiKey
- description: 'Note: We DO NOT recommend using this authentication method in production.


    With the `Uploadcare.Simple` authentication method, `auth-param` is your `public_key:secret_key` pair. Note that in this scheme, your Uploadcare project `secret_key` is  _included in every request as plain text_.


    ```http

    Accept: application/vnd.uploadcare-v0.7+json

    Authorization: Uploadcare.Simple public_key:secret_key

    ```'
  in: header
  name: Uploadcare.Simple
  parameter: Uploadcare.Simple
  sources:
  - openapi/uploadcare-rest-api-openapi.yml
  type: apiKey
slug: uploadcare-authentication
source_filename: uploadcare-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/uploadcare-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    Every request made to `https://api.uploadcare.com/` MUST be signed. HTTPS SHOULD be used with any authorization scheme.\n\n    Requests MUST contain the `Authorization` header defining `auth-scheme` and `auth-param`: `Authorization: auth-scheme auth-param`.\n\n    Every request MUST contain the `Accept` header identifying the REST API version: `Accept: application/vnd.uploadcare-v0.7+json`.\n\n    There are two ava\n  sources:\n  - openapi/uploadcare-rest-api-openapi.yml\n- name: Uploadcare\n  type: apiKey\n  in: header\n  parameter: Uploadcare\n  description: |-\n    With the `Uploadcare` authentication method:\n    * `auth-param` is a `public_key:signature` pair, where your `secret_key` is used to derive `signature`\
  \ but is _not included in every request_ itself.\n    * You MUST also provide the `Date` header in [RFC2822](https://datatracker.ietf.org/doc/html/rfc2822#section-3.3) format with the time zone set to `GMT` (see the example below).\n    * The date you provide MUST\n  sources:\n  - openapi/uploadcare-rest-api-openapi.yml\n- name: Uploadcare.Simple\n  type: apiKey\n  in: header\n  parameter: Uploadcare.Simple\n  description: |-\n    Note: We DO NOT recommend using this authentication method in production.\n\n    With the `Uploadcare.Simple` authentication method, `auth-param` is your `public_key:secret_key` pair. Note that in this scheme, your Uploadcare project `secret_key` is  _included in every request as plain text_.\n\n    ```http\n    Accept: application/vnd.uploadcare-v0.7+json\n    Authorization: Uploadcare.Simple public_key:secret_key\n    ```\n  sources:\n  - openapi/uploadcare-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uploadcare/refs/heads/main/authentication/uploadcare-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- File Upload
- File Management
- CDN
- Image Transformation
- Document Conversion
- Video Encoding
- Malware Scanning
- Storage
- Webhooks
---
