---
api_key_in:
- header
api_specs:
- filename: handy-orders-openapi.json
  format: json
  label: Handy Partner Orders API
  slug: handy-partner-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/handy/refs/heads/main/openapi/handy-orders-openapi.json
auth_types:
- signed-request
description: ''
kind: authentication
layout: security
method: searched
name: Handy Authentication
name_suffix: Authentication
oauth_flows: []
overview: handy secures its APIs with signed-request across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: handy
provider_slug: handy
scheme_count: 1
schemes:
- algorithm: RSA-SHA256 (PKCS1v15)
  example_languages:
  - python
  - javascript
  - php
  - ruby
  - java
  - csharp
  examples_repo: https://github.com/Handybook/API-Request-Signing
  headers:
  - description: The partner identifier issued by Handy.
    name: HDY-PARTNER-ID
  - description: Seconds since epoch (UTC) at request time; signed to prevent replay.
    name: HDY-TIMESTAMP
  - description: base64(rsa_sha256(private_key, PARTNER_ID + "\n" + URL + "\n" + HTTP_METHOD + "\n" + TIMESTAMP + "\n" + PAYLOAD)). RSA private key issued to the partner; Handy holds the public key.
    name: HDY-SIGNATURE
  in: header
  name: HandySignedRequest
  properties:
  - impersonation_prevented: private key never leaves the partner
  - replay_prevented: signed timestamp
  - tampering_prevented: signed payload
  scheme: rsa-sha256-signed-request
  signing_string: PARTNER_ID \n URL \n HTTP_METHOD \n TIMESTAMP \n PAYLOAD
  type: custom
slug: handy-authentication
source_filename: handy-authentication.yml
source_heading: Authentication Profile
source_url: openapi/handy-orders-openapi.json
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://partners.services.handy.com/docs/orders_api\ndocs: https://github.com/Handybook/API-Request-Signing\nsummary:\n  types: [signed-request]\n  api_key_in: [header]\n  oauth2_flows: []\n  note: >-\n    The Handy Partner API does not use a standard OpenAPI securityScheme (the\n    published Swagger declares no securityDefinitions). Authentication is a\n    custom per-request RSA-SHA256 signature scheme documented on the partner\n    docs site and in the first-party Handybook/API-Request-Signing repo.\nschemes:\n- name: HandySignedRequest\n  type: custom\n  scheme: rsa-sha256-signed-request\n  in: header\n  headers:\n  - name: HDY-PARTNER-ID\n    description: The partner identifier issued by Handy.\n  - name: HDY-TIMESTAMP\n    description: Seconds since epoch (UTC) at request time; signed to prevent replay.\n  - name: HDY-SIGNATURE\n    description: >-\n      base64(rsa_sha256(private_key, PARTNER_ID + \"\\n\" + URL + \"\
  \\n\" +\n      HTTP_METHOD + \"\\n\" + TIMESTAMP + \"\\n\" + PAYLOAD)). RSA private key issued\n      to the partner; Handy holds the public key.\n  signing_string: 'PARTNER_ID \\n URL \\n HTTP_METHOD \\n TIMESTAMP \\n PAYLOAD'\n  algorithm: RSA-SHA256 (PKCS1v15)\n  examples_repo: https://github.com/Handybook/API-Request-Signing\n  example_languages: [python, javascript, php, ruby, java, csharp]\n  properties:\n  - impersonation_prevented: private key never leaves the partner\n  - replay_prevented: signed timestamp\n  - tampering_prevented: signed payload\nonboarding:\n  contact: partners-eng@handy.com\n  note: Contact Handy partner engineering to obtain sandbox access and a keypair.\nsources:\n- openapi/handy-orders-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/handy/refs/heads/main/authentication/handy-authentication.yml
summary_line: signed-request · 1 scheme
tags:
- Company
- Home Services
- Marketplace
- Cleaning
- Handyman
- Installations
- On-Demand
- Gig Economy
- Orders
- Webhooks
- Retail
- Angi
---
