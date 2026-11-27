---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-ses-email-api-openapi.yml
  format: yaml
  label: Amazon SES Email API
  slug: amazon-ses-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-email-api-openapi.yml
- filename: amazon-ses-addon-instance-api-openapi.yml
  format: yaml
  label: Amazon SES Ses Addon Instance API
  slug: amazon-ses-addon-instance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-addon-instance-api-openapi.yml
- filename: amazon-ses-addon-subscription-api-openapi.yml
  format: yaml
  label: Amazon SES Ses Addon Subscription API
  slug: amazon-ses-addon-subscription-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-addon-subscription-api-openapi.yml
- filename: amazon-ses-address-list-api-openapi.yml
  format: yaml
  label: Amazon SES Ses Address List API
  slug: amazon-ses-address-list-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-address-list-api-openapi.yml
- filename: amazon-ses-address-list-import-job-api-openapi.yml
  format: yaml
  label: Amazon SES Ses Address List Import Job API
  slug: amazon-ses-address-list-import-job-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-address-list-import-job-api-openapi.yml
- filename: amazon-ses-archive-api-openapi.yml
  format: yaml
  label: Amazon SES Ses Archive API
  slug: amazon-ses-archive-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-archive-api-openapi.yml
- filename: amazon-ses-archive-export-api-openapi.yml
  format: yaml
  label: Amazon SES Ses Archive Export API
  slug: amazon-ses-archive-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-archive-export-api-openapi.yml
- filename: amazon-ses-archive-search-api-openapi.yml
  format: yaml
  label: Amazon SES Ses Archive Search API
  slug: amazon-ses-archive-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-archive-search-api-openapi.yml
- filename: amazon-ses-configuration-set-tracking-option-api-openapi.yml
  format: yaml
  label: Amazon SES Ses Configuration Set Tracking Option API
  slug: amazon-ses-configuration-set-tracking-option-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-configuration-set-tracking-option-api-openapi.yml
- filename: amazon-ses-identity-policy-api-openapi.yml
  format: yaml
  label: Amazon SES Ses Identity Policy API
  slug: amazon-ses-identity-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-identity-policy-api-openapi.yml
- filename: amazon-ses-ingress-point-api-openapi.yml
  format: yaml
  label: Amazon SES Ses Ingress Point API
  slug: amazon-ses-ingress-point-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-ingress-point-api-openapi.yml
- filename: amazon-ses-operations-api-openapi.yml
  format: yaml
  label: Amazon SES Ses Operations API
  slug: amazon-ses-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-operations-api-openapi.yml
- filename: amazon-ses-receipt-filter-api-openapi.yml
  format: yaml
  label: Amazon SES Ses Receipt Filter API
  slug: amazon-ses-receipt-filter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-receipt-filter-api-openapi.yml
- filename: amazon-ses-receipt-rule-api-openapi.yml
  format: yaml
  label: Amazon SES Ses Receipt Rule API
  slug: amazon-ses-receipt-rule-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-receipt-rule-api-openapi.yml
- filename: amazon-ses-receipt-rule-set-api-openapi.yml
  format: yaml
  label: Amazon SES Ses Receipt Rule Set API
  slug: amazon-ses-receipt-rule-set-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-receipt-rule-set-api-openapi.yml
- filename: amazon-ses-relay-api-openapi.yml
  format: yaml
  label: Amazon SES Ses Relay API
  slug: amazon-ses-relay-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-relay-api-openapi.yml
- filename: amazon-ses-rule-set-api-openapi.yml
  format: yaml
  label: Amazon SES Ses Rule Set API
  slug: amazon-ses-rule-set-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-rule-set-api-openapi.yml
- filename: amazon-ses-template-api-openapi.yml
  format: yaml
  label: Amazon SES Ses Template API
  slug: amazon-ses-template-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-template-api-openapi.yml
- filename: amazon-ses-traffic-policy-api-openapi.yml
  format: yaml
  label: Amazon SES Ses Traffic Policy API
  slug: amazon-ses-traffic-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-traffic-policy-api-openapi.yml
auth_types:
- apiKey
- sigv4
- smtp-credentials
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Amazon SES Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon SES secures its APIs with apiKey, sigv4, and smtp-credentials across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon SES
provider_slug: amazon-ses
scheme_count: 1
schemes:
- applied: global
  description: Amazon Signature Version 4 (SigV4)
  in: header
  name: hmac
  note: Declared as type apiKey in the spec because OpenAPI 3.0 has no native SigV4 scheme. It is not a static API key — the Authorization header carries a request signature computed per request from the AWS access key id, secret access key, region, service name (ses) and a canonical request hash.
  parameter: Authorization
  sources:
  - openapi/_superseded/amazon-ses-sesv2-openapi.yml
  type: apiKey
  x_amazon_apigateway_authtype: awsSigv4
slug: amazon-ses-authentication
source_filename: amazon-ses-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/_superseded/amazon-ses-sesv2-openapi.yml\ndocs: https://docs.aws.amazon.com/ses/latest/dg/security-iam.html\nnote: >-\n  0-working/derive-authentication.py returned zero profiles for this repo because it scans only the top-level\n  openapi/ directory and the four refined SES specs carry no securitySchemes block. The scheme below was read\n  from the harvested SES v2 spec in openapi/_original/ and enriched from the AWS docs, so this file is\n  method: searched rather than derived.\nsummary:\n  types: [apiKey, sigv4, smtp-credentials]\n  api_key_in: [header]\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\nschemes:\n  - name: hmac\n    type: apiKey\n    in: header\n    parameter: Authorization\n    description: Amazon Signature Version 4 (SigV4)\n    x_amazon_apigateway_authtype: awsSigv4\n    sources: [openapi/_superseded/amazon-ses-sesv2-openapi.yml]\n    applied: global\n    note:\
  \ >-\n      Declared as type apiKey in the spec because OpenAPI 3.0 has no native SigV4 scheme. It is not a static\n      API key — the Authorization header carries a request signature computed per request from the AWS access\n      key id, secret access key, region, service name (ses) and a canonical request hash.\nmodel:\n  primary: AWS Signature Version 4\n  credential_source: AWS IAM (long-lived access keys, or short-lived STS credentials from an assumed role)\n  request_headers:\n    - Authorization\n    - X-Amz-Date\n    - X-Amz-Content-Sha256\n    - X-Amz-Security-Token\n  signing_service_name: ses\n  regional: true\n  note: The credential scope embeds the AWS Region, so a signature is valid only for the region it was signed for.\nalternatives:\n  - name: SMTP interface\n    mechanism: SES SMTP credentials (an SMTP username/password pair derived from an IAM user's credentials)\n    endpoints: email-smtp.{region}.amazonaws.com\n    ports: [25, 465, 587, 2465, 2587]\n    transport_security:\
  \ STARTTLS on 25/587/2587, TLS Wrapper on 465/2465\n    docs: https://docs.aws.amazon.com/ses/latest/dg/smtp-credentials.html\n    note: >-\n      SMTP credentials are NOT the IAM secret access key. They are derived from it with a documented\n      algorithm and must be generated explicitly; an IAM secret key pasted into an SMTP client will fail.\n  - name: Sending authorization policies\n    mechanism: Resource policy attached to a verified identity, delegating send rights to another AWS account\n    operations: [CreateEmailIdentityPolicy, UpdateEmailIdentityPolicy, DeleteEmailIdentityPolicy, GetEmailIdentityPolicies]\n    docs: https://docs.aws.amazon.com/ses/latest/dg/sending-authorization.html\nauthorization:\n  model: AWS IAM policies\n  action_prefix: 'ses:'\n  granularity: per-operation IAM actions, with resource-level conditions on identities, configuration sets and templates\n  condition_keys:\n    - 'ses:Recipients'\n    - 'ses:FromAddress'\n    - 'ses:FromDisplayName'\n    -\
  \ 'ses:FeedbackAddress'\n    - 'ses:FromArn'\n  docs: https://docs.aws.amazon.com/ses/latest/dg/security_iam_service-with-iam.html\n  note: >-\n    SES has no OAuth scope surface. Authorization is expressed entirely in IAM policy, which is why no\n    scopes/ artifact is emitted for this provider.\noauth:\n  supported: false\n  evidence: >-\n    No oauth2 securityScheme in any harvested SES spec; https://aws.amazon.com/.well-known/oauth-authorization-server\n    and /.well-known/openid-configuration both returned 404 when probed 2026-08-13.\n"
source_yaml_url: https://artifacts.apis.io/amazon-ses/authentication/amazon-ses-authentication.yml
summary_line: apiKey/sigv4/smtp-credentials · 1 scheme
tags:
- Amazon Web Services
- Email
- Email Deliverability
- Email Service
- Marketing Email
- Notification
- SMTP
- Transactional Email
- Bulk Email
- Email Receiving
- DKIM
- Messaging
- Cloud Infrastructure
---
