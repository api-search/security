---
api_key_in:
- header
auth_types:
- apiKey
- hmac-signature
description: ''
kind: authentication
layout: security
method: searched
name: Qiniu Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qiniu Cloud secures its APIs with apiKey and hmac-signature across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Qiniu Cloud
provider_slug: qiniu
scheme_count: 3
schemes:
- algorithm: HMAC-SHA1
  description: Management/access token. Signs the HTTP method, path, query, host, selected headers and body with the SecretKey, URL-safe-base64 encodes it, and concatenates it with the AccessKey. Used for resource-management operations (delete/move/copy, bucket admin, IAM). Invalid signatures return HTTP 401.
  encoding: url-safe base64
  header: 'Authorization: Qiniu <AccessKey>:<EncodedSign>'
  name: Qiniu
  type: hmac-signature
- algorithm: HMAC-SHA1
  description: Legacy management token variant signing path + query + body. Still accepted by many management endpoints; the newer Qiniu signature is recommended.
  header: 'Authorization: QBox <AccessKey>:<EncodedSign>'
  name: QBox
  type: hmac-signature
- description: Scoped, expiring token minted client-side from AK/SK for a specific bucket (and optional key/policy). Presented on upload requests to the up.* hosts. Carries a PutPolicy (scope, deadline, callback, returnBody, mimeLimit, etc.).
  header: 'Authorization: UpToken <token> (or multipart token field)'
  name: UploadToken
  type: token
slug: qiniu-authentication
source_filename: qiniu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developer.qiniu.com/kodo/1201/access-token\ndocs: https://developer.qiniu.com/kodo/1201/access-token\nsummary:\n  types: [apiKey, hmac-signature]\n  credential: AccessKey / SecretKey (AK/SK)\n  credential_source: https://portal.qiniu.com (console -> key management)\n  api_key_in: [header]\nschemes:\n  - name: Qiniu\n    type: hmac-signature\n    algorithm: HMAC-SHA1\n    header: 'Authorization: Qiniu <AccessKey>:<EncodedSign>'\n    description: >-\n      Management/access token. Signs the HTTP method, path, query, host, selected\n      headers and body with the SecretKey, URL-safe-base64 encodes it, and\n      concatenates it with the AccessKey. Used for resource-management operations\n      (delete/move/copy, bucket admin, IAM). Invalid signatures return HTTP 401.\n    encoding: url-safe base64\n  - name: QBox\n    type: hmac-signature\n    algorithm: HMAC-SHA1\n    header: 'Authorization: QBox <AccessKey>:<EncodedSign>'\n\
  \    description: >-\n      Legacy management token variant signing path + query + body. Still accepted\n      by many management endpoints; the newer Qiniu signature is recommended.\n  - name: UploadToken\n    type: token\n    description: >-\n      Scoped, expiring token minted client-side from AK/SK for a specific bucket\n      (and optional key/policy). Presented on upload requests to the up.* hosts.\n      Carries a PutPolicy (scope, deadline, callback, returnBody, mimeLimit, etc.).\n    header: 'Authorization: UpToken <token> (or multipart token field)'\nnotes: >-\n  Qiniu has no OAuth2/OIDC surface — there is no scope reference and no\n  /.well-known discovery. All authentication derives from the account AK/SK pair;\n  IAM sub-accounts get their own AK/SK keypairs with policy-based permissions.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qiniu/refs/heads/main/authentication/qiniu-authentication.yml
summary_line: apiKey/hmac-signature · 3 schemes
tags:
- Company
- Cloud
- Object Storage
- CDN
- Media Processing
- Live Streaming
- IAM
- SDK
- AI
- China
---
