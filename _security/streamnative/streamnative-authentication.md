---
anonymous_access: false
api_key_in: []
api_specs:
- filename: streamnative-cloudstreamnativeio-v1alpha1-api-openapi.yml
  format: yaml
  label: StreamNative Cloud Streamnative Io V1alpha1 API
  slug: streamnative-cloudstreamnativeio-v1alpha1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streamnative/refs/heads/main/openapi/streamnative-cloudstreamnativeio-v1alpha1-api-openapi.yml
- filename: streamnative-ksn-consumer-group-api-openapi.yml
  format: yaml
  label: StreamNative Ksn Consumer Group API
  slug: streamnative-ksn-consumer-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streamnative/refs/heads/main/openapi/streamnative-ksn-consumer-group-api-openapi.yml
- filename: streamnative-ksn-topics-api-openapi.yml
  format: yaml
  label: StreamNative Ksn Topics API
  slug: streamnative-ksn-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streamnative/refs/heads/main/openapi/streamnative-ksn-topics-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Streamnative Authentication
name_suffix: Authentication
oauth_flows: []
overview: StreamNative declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: StreamNative
provider_slug: streamnative
scheme_count: 2
schemes:
- applies_to:
  - StreamNative Cloud API
  flow: clientCredentials
  name: oauth2ClientCredentials
  tokenUrl: https://auth.streamnative.cloud/oauth/token
  type: oauth2
- applies_to:
  - StreamNative Kafka REST API
  name: bearerToken
  scheme: bearer
  source: https://docs.streamnative.io/cloud/build/kafka-clients/kafka-rest-api
  type: http
slug: streamnative-authentication
source_filename: streamnative-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: searched\nsource: https://docs.streamnative.io/api-references/cloudapi/cloud-api\ndocs: https://docs.streamnative.io/api-references/cloudapi/cloud-api\nsummary: >-\n  \"StreamNative cloud supports OAuth2 authentication to managing cloud resources.\" The Cloud API uses the\n  OAuth2 client credential flow against https://auth.streamnative.cloud/oauth/token with a service account\n  downloaded from the console; the Kafka REST API is called with 'Authorization: Bearer <your-token>'.\nschemes:\n- name: oauth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  tokenUrl: https://auth.streamnative.cloud/oauth/token\n  applies_to: [StreamNative Cloud API]\n- name: bearerToken\n  type: http\n  scheme: bearer\n  applies_to: [StreamNative Kafka REST API]\n  source: https://docs.streamnative.io/cloud/build/kafka-clients/kafka-rest-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/streamnative/refs/heads/main/authentication/streamnative-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Data Streaming
- Apache Pulsar
- Apache Kafka
- Messaging
- Event Streaming
- Cloud
---
