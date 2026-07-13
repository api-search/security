---
api_key_in: []
api_specs:
- filename: enable-banking-api-openapi.yml
  format: yaml
  label: Enable Banking API
  slug: enable-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enable-banking/refs/heads/main/openapi/enable-banking-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Enable Banking Authentication
name_suffix: Authentication
oauth_flows: []
overview: Enable Banking secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Enable Banking
provider_slug: enable-banking
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'In order to get access to this API you need to:


    - Generate a private RSA key and a self-signed certificate;

    - Upload the certificate to enablebanking.com and get application ID;

    - Construct JWT with the data described below and signed with your private key;

    - Send the JWT in the Authorization header.


    ## Private key and certificate generation


    > Generating private RSA key


    ```bash

    openssl genrsa '
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/enable-banking-api-openapi.yml
  type: http
slug: enable-banking-authentication
source_filename: enable-banking-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/enable-banking-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: \"In order to get access to this API you need to:\\n\\n- Generate a private RSA\\\n    \\ key and a self-signed certificate;\\n- Upload the certificate to enablebanking.com and\\\n    \\ get application ID;\\n- Construct JWT with the data described below and signed with your\\\n    \\ private key;\\n- Send the JWT in the Authorization header.\\n\\n## Private key and certificate\\\n    \\ generation\\n\\n> Generating private RSA key\\n\\n```bash\\nopenssl genrsa \"\n  sources:\n  - openapi/enable-banking-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enable-banking/refs/heads/main/authentication/enable-banking-authentication.yml
summary_line: http · 1 scheme
tags:
- Open Banking
- PSD2
- AISP
- PISP
- Banking
- Financial Services
- Account Aggregation
- Payment Initiation
- Europe
- Nordic
- Finland
- Compliance
- eIDAS
- SCA
- DORA
- GDPR
---
