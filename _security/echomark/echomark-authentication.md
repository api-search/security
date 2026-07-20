---
api_key_in: []
auth_types:
- apiClientCredentials
description: ''
kind: authentication
layout: security
method: searched
name: Echomark Authentication
name_suffix: Authentication
oauth_flows: []
overview: EchoMark secures its APIs with apiClientCredentials across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: EchoMark
provider_slug: echomark
scheme_count: 1
schemes:
- description: API access is authenticated with API client credentials. Per the EchoMark API product page, administrators "Create API clients in the EchoMark web application. No request form, no manual approval required." The exact wire format (header name / bearer vs. key) is documented in the support portal API reference and is not published on the public marketing surface, so it is not asserted here.
  name: EchoMarkAPIClient
  sources:
  - https://www.echomark.com/product/api
  type: apiClientCredentials
slug: echomark-authentication
source_filename: echomark-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.echomark.com/product/api\ndocs: https://support.echomark.com/hc/en-us/sections/48912786989332-EchoMark-API\nsummary:\n  types:\n  - apiClientCredentials\n  self_service: true\nschemes:\n- name: EchoMarkAPIClient\n  type: apiClientCredentials\n  description: >-\n    API access is authenticated with API client credentials. Per the EchoMark API\n    product page, administrators \"Create API clients in the EchoMark web application.\n    No request form, no manual approval required.\" The exact wire format (header name /\n    bearer vs. key) is documented in the support portal API reference and is not\n    published on the public marketing surface, so it is not asserted here.\n  sources:\n  - https://www.echomark.com/product/api\nnotes: >-\n  Derived from public marketing docs only (no public OpenAPI). API clients are created\n  self-service in the web app at https://app.echomark.com. Upgrade with the support-portal\n\
  \  API reference when accessible.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/echomark/refs/heads/main/authentication/echomark-authentication.yml
summary_line: apiClientCredentials · 1 scheme
tags:
- Company
- Security
- Information Security
- Forensic Watermarking
- Insider Threat
- Data Loss Prevention
- Leak Detection
---
