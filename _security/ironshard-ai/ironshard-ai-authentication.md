---
anonymous_access: false
api_key_in: []
auth_types: []
description: IronShard S3 API uses AWS Signature Version 4 with an access key and secret key.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: IronShard Authentication
name_suffix: Authentication
oauth_flows: []
overview: IronShard declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: IronShard
provider_slug: ironshard-ai
scheme_count: 1
schemes:
- evidence: 'Credentials file Environment variables ~/.aws/credentials : [ironshard] aws_access_key_id = IRONSHARD_ACCESS_KEY aws_secret_access_key = IRONSHARD_SECRET_KEY'
  header: Authorization
  how_to_obtain: Create an Access Key in the console (S3 Access Keys → New Key).
  location: header
  name: aws_access_key_id / aws_secret_access_key
  type: apiKey
slug: ironshard-ai-authentication
source_filename: ironshard-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://www.ironshard.ai/docs/s3-quickstart
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.ironshard.ai/docs/s3-quickstart\nsources:\n- https://www.ironshard.ai/docs/s3-quickstart\ndescription: IronShard S3 API uses AWS Signature Version 4 with an access key and secret key.\nschemes:\n- type: apiKey\n  name: aws_access_key_id / aws_secret_access_key\n  evidence: 'Credentials file Environment variables ~/.aws/credentials : [ironshard] aws_access_key_id = IRONSHARD_ACCESS_KEY aws_secret_access_key\n    = IRONSHARD_SECRET_KEY'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an Access Key in the console (S3 Access Keys → New Key).\nnote: No OAuth2, http‑basic, http‑bearer, jwt, hmac, mtls, or other schemes are documented on the page.\ndocs: https://www.ironshard.ai/docs/s3-quickstart\n"
source_yaml_url: https://artifacts.apis.io/ironshard-ai/authentication/ironshard-ai-authentication.yml
summary_line: 1 scheme
tags:
- Storage
- Artificial Intelligence
- Cloud
- S3
- MCP
---
