---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-cloudtrail-event-data-stores-api-openapi.yml
  format: yaml
  label: Amazon CloudTrail Event Data Stores API
  slug: amazon-cloudtrail-event-data-stores-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudtrail/openapi/amazon-cloudtrail-event-data-stores-api-openapi.yml
- filename: amazon-cloudtrail-events-api-openapi.yml
  format: yaml
  label: Amazon CloudTrail Events API
  slug: amazon-cloudtrail-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudtrail/openapi/amazon-cloudtrail-events-api-openapi.yml
- filename: amazon-cloudtrail-trails-api-openapi.yml
  format: yaml
  label: Amazon CloudTrail Trails API
  slug: amazon-cloudtrail-trails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudtrail/openapi/amazon-cloudtrail-trails-api-openapi.yml
- filename: amazon-cloudtrail-channel-api-openapi.yml
  format: yaml
  label: Amazon CloudTrail Cloudtrail Channel API
  slug: amazon-cloudtrail-channel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudtrail/openapi/amazon-cloudtrail-channel-api-openapi.yml
- filename: amazon-cloudtrail-dashboard-api-openapi.yml
  format: yaml
  label: Amazon CloudTrail Cloudtrail Dashboard API
  slug: amazon-cloudtrail-dashboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudtrail/openapi/amazon-cloudtrail-dashboard-api-openapi.yml
- filename: amazon-cloudtrail-import-api-openapi.yml
  format: yaml
  label: Amazon CloudTrail Cloudtrail Import API
  slug: amazon-cloudtrail-import-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudtrail/openapi/amazon-cloudtrail-import-api-openapi.yml
- filename: amazon-cloudtrail-operations-api-openapi.yml
  format: yaml
  label: Amazon CloudTrail Cloudtrail Operations API
  slug: amazon-cloudtrail-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudtrail/openapi/amazon-cloudtrail-operations-api-openapi.yml
- filename: amazon-cloudtrail-query-api-openapi.yml
  format: yaml
  label: Amazon CloudTrail Cloudtrail Query API
  slug: amazon-cloudtrail-query-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudtrail/openapi/amazon-cloudtrail-query-api-openapi.yml
- filename: amazon-cloudtrail-resource-policy-api-openapi.yml
  format: yaml
  label: Amazon CloudTrail Cloudtrail Resource Policy API
  slug: amazon-cloudtrail-resource-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudtrail/openapi/amazon-cloudtrail-resource-policy-api-openapi.yml
- filename: amazon-cloudtrail-tag-api-openapi.yml
  format: yaml
  label: Amazon CloudTrail Cloudtrail Tag API
  slug: amazon-cloudtrail-tag-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-cloudtrail/openapi/amazon-cloudtrail-tag-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon CloudTrail Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon CloudTrail secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon CloudTrail
provider_slug: amazon-cloudtrail
scheme_count: 1
schemes:
- description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256 signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary credentials). Not a bearer token.
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-cloudtrail-channel-api-openapi.yml
  - openapi/amazon-cloudtrail-dashboard-api-openapi.yml
  - openapi/amazon-cloudtrail-event-data-stores-api-openapi.yml
  - openapi/amazon-cloudtrail-events-api-openapi.yml
  - openapi/amazon-cloudtrail-import-api-openapi.yml
  - openapi/amazon-cloudtrail-operations-api-openapi.yml
  - openapi/amazon-cloudtrail-query-api-openapi.yml
  - openapi/amazon-cloudtrail-resource-policy-api-openapi.yml
  - openapi/amazon-cloudtrail-tag-api-openapi.yml
  - openapi/amazon-cloudtrail-trails-api-openapi.yml
  type: apiKey
slug: amazon-cloudtrail-authentication
source_filename: amazon-cloudtrail-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/amazon-cloudtrail-channel-api-openapi.yml, openapi/amazon-cloudtrail-dashboard-api-openapi.yml,\n  openapi/amazon-cloudtrail-event-data-stores-api-openapi.yml, openapi/amazon-cloudtrail-events-api-openapi.yml,\n  openapi/amazon-cloudtrail-import-api-openapi.yml, openapi/amazon-cloudtrail-operations-api-openapi.yml,\n  openapi/amazon-cloudtrail-query-api-openapi.yml, openapi/amazon-cloudtrail-resource-policy-api-openapi.yml,\n  openapi/amazon-cloudtrail-tag-api-openapi.yml, openapi/amazon-cloudtrail-trails-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256\n    signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary\n    credentials). Not a bearer token.\n  sources:\n  - openapi/amazon-cloudtrail-channel-api-openapi.yml\n\
  \  - openapi/amazon-cloudtrail-dashboard-api-openapi.yml\n  - openapi/amazon-cloudtrail-event-data-stores-api-openapi.yml\n  - openapi/amazon-cloudtrail-events-api-openapi.yml\n  - openapi/amazon-cloudtrail-import-api-openapi.yml\n  - openapi/amazon-cloudtrail-operations-api-openapi.yml\n  - openapi/amazon-cloudtrail-query-api-openapi.yml\n  - openapi/amazon-cloudtrail-resource-policy-api-openapi.yml\n  - openapi/amazon-cloudtrail-tag-api-openapi.yml\n  - openapi/amazon-cloudtrail-trails-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-cloudtrail/authentication/amazon-cloudtrail-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Web Services
- CloudTrail
- Audit
- Compliance
- Governance
- Security
---
