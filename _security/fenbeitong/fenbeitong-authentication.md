---
api_key_in:
- body
auth_types:
- token
- signature
description: ''
kind: authentication
layout: security
method: searched
name: Fenbeitong Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fenbeitong secures its APIs with token and signature across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Fenbeitong
provider_slug: fenbeitong
scheme_count: 2
schemes:
- description: Exchange app_id + app_key for a short-lived JWT access_token. Token is valid for 2 hours; re-request on expiry.
  name: TokenDispense
  request:
    content_type: application/x-www-form-urlencoded
    method: POST
    parameters:
    - description: Enterprise ID (企业ID)
      name: app_id
      required: true
    - description: Enterprise key (企业key)
      name: app_key
      required: true
    - description: Reserved field (预留字段)
      name: app_type
      required: false
    path: /open/api/auth/v1/dispense
  response_envelope:
    code: 0 = success
    data.access_token: JWT bearer token (JWT HS256), 2-hour TTL
    msg: status message
    request_id: correlation id
  token_format: JWT (alg HS256)
  token_ttl_seconds: 7200
  type: token
- algorithm: md5-hex
  description: Business requests are signed with an MD5-hex signature over the timestamp, the JSON request body (data), and the enterprise sign_key. The sign_key is a shared secret that participates in the signature but is never sent on the wire.
  name: RequestSignature
  parameters:
  - description: 13-digit epoch-millis timestamp
    name: timestamp
  - description: JSON business payload
    name: data
  - description: Enterprise-issued shared secret; not transmitted
    name: sign_key
  reference_impl: org.apache.commons.codec.digest.DigestUtils.md5Hex(bytes)
  signed_string_template: timestamp={timestamp}&data={jsonData}&sign_key={signKey}
  type: signature
slug: fenbeitong-authentication
source_filename: fenbeitong-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: http://docs.open.fenbeitong.com/open-api/2apijie-ru/23-jian-quan-jie-kou-ff0c-ban-fa-token.html\ndocs: http://docs.open.fenbeitong.com/open-api/1.fenbeitong-introduction.html\nsummary:\n  model: app-credentials + bearer-token + request-signature\n  types:\n  - token\n  - signature\n  api_key_in:\n  - body\n  oauth2_flows: []\n  notes: >-\n    Fenbeitong Open Platform (开放平台) is NOT OAuth2. Access is granted to\n    enterprises that have a business relationship with Fenbeitong. Onboarding\n    issues three credentials — app_id (企业ID), app_key (企业key), and sign_key\n    (issued but NEVER transmitted, used only to compute the request signature).\nschemes:\n- name: TokenDispense\n  type: token\n  description: >-\n    Exchange app_id + app_key for a short-lived JWT access_token. Token is\n    valid for 2 hours; re-request on expiry.\n  request:\n    method: POST\n    path: /open/api/auth/v1/dispense\n    content_type: application/x-www-form-urlencoded\n\
  \    parameters:\n    - name: app_id\n      required: true\n      description: Enterprise ID (企业ID)\n    - name: app_key\n      required: true\n      description: Enterprise key (企业key)\n    - name: app_type\n      required: false\n      description: Reserved field (预留字段)\n  response_envelope:\n    request_id: correlation id\n    code: 0 = success\n    msg: status message\n    data.access_token: JWT bearer token (JWT HS256), 2-hour TTL\n  token_format: JWT (alg HS256)\n  token_ttl_seconds: 7200\n- name: RequestSignature\n  type: signature\n  description: >-\n    Business requests are signed with an MD5-hex signature over the timestamp,\n    the JSON request body (data), and the enterprise sign_key. The sign_key is\n    a shared secret that participates in the signature but is never sent on the\n    wire.\n  algorithm: md5-hex\n  signed_string_template: timestamp={timestamp}&data={jsonData}&sign_key={signKey}\n  parameters:\n  - name: timestamp\n    description: 13-digit epoch-millis timestamp\n\
  \  - name: data\n    description: JSON business payload\n  - name: sign_key\n    description: Enterprise-issued shared secret; not transmitted\n  reference_impl: org.apache.commons.codec.digest.DigestUtils.md5Hex(bytes)\nenvironments:\n- name: production\n  host: https://open.fenbeitong.com\n- name: sandbox\n  host: https://open-sandbox.fenbeitong.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fenbeitong/refs/heads/main/authentication/fenbeitong-authentication.yml
summary_line: token/signature · 2 schemes
tags:
- Company
- Fintech
- Spend Management
- Expense Management
- Corporate Travel
- Payments
- Procurement
- China
---
