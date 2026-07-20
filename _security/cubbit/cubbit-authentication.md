---
api_key_in:
- signed-request
auth_types:
- awsSigV4
description: 'Authentication profile for the Cubbit DS3 S3-compatible API. DS3 uses AWS S3 authentication: an access key ID and secret access key signed with AWS Signature Version 4. Credentials are created per project in the DS3 web console (Access key menu) and downloaded as a CSV. There is no OAuth surface on the storage API itself (the console login uses a separate OIDC flow that is not the API auth mechanism).'
kind: authentication
layout: security
method: searched
name: Cubbit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cubbit secures its APIs with awsSigV4 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cubbit
provider_slug: cubbit
scheme_count: 1
schemes:
- credential_source: DS3 web console (console.cubbit.eu) → project → Access key → Create access key
  description: AWS Signature Version 4 request signing using an access key ID and secret access key, identical to Amazon S3. Compatible with the AWS SDKs and AWS CLI when pointed at the s3.cubbit.eu endpoint.
  endpoint: https://s3.cubbit.eu
  name: AWSSignatureV4
  region: eu-west-1
  scheme: aws-sigv4
  sources:
  - docs.cubbit.io/getting-started/quickstart
  - docs.cubbit.io/guides/s3-api
  type: awsSigV4
slug: cubbit-authentication
source_filename: cubbit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.cubbit.io/getting-started/quickstart\ndocs: https://docs.cubbit.io/guides/s3-api\ndescription: >-\n  Authentication profile for the Cubbit DS3 S3-compatible API. DS3 uses AWS S3\n  authentication: an access key ID and secret access key signed with AWS\n  Signature Version 4. Credentials are created per project in the DS3 web\n  console (Access key menu) and downloaded as a CSV. There is no OAuth surface\n  on the storage API itself (the console login uses a separate OIDC flow that is\n  not the API auth mechanism).\nsummary:\n  types: [awsSigV4]\n  api_key_in: [signed-request]\n  oauth2_flows: []\nschemes:\n- name: AWSSignatureV4\n  type: awsSigV4\n  scheme: aws-sigv4\n  description: >-\n    AWS Signature Version 4 request signing using an access key ID and secret\n    access key, identical to Amazon S3. Compatible with the AWS SDKs and AWS CLI\n    when pointed at the s3.cubbit.eu endpoint.\n  region: eu-west-1\n\
  \  endpoint: https://s3.cubbit.eu\n  credential_source: DS3 web console (console.cubbit.eu) → project → Access key → Create access key\n  sources: [docs.cubbit.io/getting-started/quickstart, docs.cubbit.io/guides/s3-api]\nnotes:\n- Custom tenants sign against https://s3.<tenant>.cubbit.eu.\n- Secret access keys are shown once at creation and downloaded as CSV.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cubbit/refs/heads/main/authentication/cubbit-authentication.yml
summary_line: awsSigV4 · 1 scheme
tags:
- Object Storage
- Cloud Storage
- S3 Compatible
- Storage
- Data Sovereignty
- Geo-Distributed
- Infrastructure
- Company
---
