---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Easyar Crs Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: EasyAR CRS API declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: EasyAR CRS API
provider_slug: easyar-crs-api
scheme_count: 2
schemes:
- description: 'Temporary access token placed in the HTTP Authorization header. Tokens are issued either from the EasyAR development center UI or programmatically from the STS (Security Token Service) by signing apiKey + expires + acl + timestamp with the API Secret (sha256 of sorted key+value concatenation with the secret appended). The acl grants per-service, per-resource, per-permission access, e.g. {service: "ecs:crs", resource: ["<CRS AppId>"], effect: "Allow", permission: ["READ"]}. Tokens expire after the requested validity window (expires, in seconds).'
  docs: https://www.easyar.com/doc/en/develop/apikey-auth.html#api-token
  header: Authorization
  in: header
  name: apiKeyToken
  type: token
- description: Signature authentication carries appId (or legacy appKey), timestamp (milliseconds), apiKey and signature as common request parameters instead of an Authorization header. All parameters except image binaries are included in the signature calculation; the signature is the hex sha256 of the sorted key+value concatenation with the API Secret appended.
  docs: https://www.easyar.com/doc/en/api/cloud/cloud-recognition/apis.html
  in: query-or-body
  name: requestSignature
  type: signature
slug: easyar-crs-api-authentication
source_filename: easyar-crs-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: searched\nsource: https://www.easyar.com/doc/en/develop/apikey-auth.html\ndocs: https://www.easyar.com/doc/en/develop/apikey-auth.html\nnote: >-\n  No OpenAPI is published, so this profile is written from the provider's own authentication docs\n  (Get and use API Key; Introduction to cloud recognition APIs). EasyAR cloud services (CRS cloud\n  recognition, Sparse SpatialMap, Mega Block localization) share one unified API Key system.\nschemes:\n  - name: apiKeyToken\n    type: token\n    in: header\n    header: Authorization\n    description: >-\n      Temporary access token placed in the HTTP Authorization header. Tokens are issued either from\n      the EasyAR development center UI or programmatically from the STS (Security Token Service) by\n      signing apiKey + expires + acl + timestamp with the API Secret (sha256 of sorted key+value\n      concatenation with the secret appended). The acl grants per-service, per-resource, per-permission\n\
  \      access, e.g. {service: \"ecs:crs\", resource: [\"<CRS AppId>\"], effect: \"Allow\", permission: [\"READ\"]}.\n      Tokens expire after the requested validity window (expires, in seconds).\n    docs: https://www.easyar.com/doc/en/develop/apikey-auth.html#api-token\n  - name: requestSignature\n    type: signature\n    in: query-or-body\n    description: >-\n      Signature authentication carries appId (or legacy appKey), timestamp (milliseconds), apiKey and\n      signature as common request parameters instead of an Authorization header. All parameters except\n      image binaries are included in the signature calculation; the signature is the hex sha256 of the\n      sorted key+value concatenation with the API Secret appended.\n    docs: https://www.easyar.com/doc/en/api/cloud/cloud-recognition/apis.html\ntoken_service:\n  name: UAC / STS token exchange\n  url: https://uac.easyar.com/token/v2\n  note: >-\n    The docs' management checklist points at \"the UAC API — Create Token\
  \ method, using the original\n    APIKey and APISecret to create a Token\". No standalone public reference page for the UAC endpoint\n    exists in the English doc sitemap; signing examples in PHP/JS/Python/Java/C#/Go are published on\n    the apikey-auth page. A blank POST to https://uac.easyar.com/token/v2 answers HTTP 400 (live host).\nacl:\n  services: [\"ecs:crs\", \"ecs:spatialmap\", \"ecs:cls\", \"ecs:vps1\"]\n  effects: [\"Allow\", \"Deny\"]\n  permissions: [\"READ\", \"WRITE\"]\nwarnings:\n  - Do not use API Key and API Secret directly in client applications (Web, WeChat Mini Programs).\n  - Generate tokens server-side and pass them to the client.\noauth2: false\nopenid_connect: false\nmutual_tls: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/easyar-crs-api/refs/heads/main/authentication/easyar-crs-api-authentication.yml
summary_line: 2 schemes
tags:
- Augmented Reality
- ar-sdk
- Cloud Recognition
- Image Recognition
- Spatial Computing
- Visual Positioning
- Computer-Vision
- Developer Tools
---
