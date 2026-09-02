---
api_specs:
- filename: amazon-sns-action-listtagsforresource-api-openapi.yml
  format: yaml
  label: Amazon SNS ?Action=ListTagsForResource API
  slug: amazon-sns-action-listtagsforresource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-sns/refs/heads/main/openapi/amazon-sns-action-listtagsforresource-api-openapi.yml
- filename: amazon-sns-action-tagresource-api-openapi.yml
  format: yaml
  label: Amazon SNS ?Action=TagResource API
  slug: amazon-sns-action-tagresource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-sns/refs/heads/main/openapi/amazon-sns-action-tagresource-api-openapi.yml
- filename: amazon-sns-action-untagresource-api-openapi.yml
  format: yaml
  label: Amazon SNS ?Action=UntagResource API
  slug: amazon-sns-action-untagresource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-sns/refs/heads/main/openapi/amazon-sns-action-untagresource-api-openapi.yml
- filename: amazon-sns-platform-applications-api-openapi.yml
  format: yaml
  label: Amazon SNS Platform Applications API
  slug: amazon-sns-platform-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-sns/refs/heads/main/openapi/amazon-sns-platform-applications-api-openapi.yml
- filename: amazon-sns-publishing-api-openapi.yml
  format: yaml
  label: Amazon SNS Publishing API
  slug: amazon-sns-publishing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-sns/refs/heads/main/openapi/amazon-sns-publishing-api-openapi.yml
- filename: amazon-sns-sms-api-openapi.yml
  format: yaml
  label: Amazon SNS SMS API
  slug: amazon-sns-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-sns/refs/heads/main/openapi/amazon-sns-sms-api-openapi.yml
- filename: amazon-sns-subscriptions-api-openapi.yml
  format: yaml
  label: Amazon SNS Subscriptions API
  slug: amazon-sns-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-sns/refs/heads/main/openapi/amazon-sns-subscriptions-api-openapi.yml
- filename: amazon-sns-topics-api-openapi.yml
  format: yaml
  label: Amazon SNS Topics API
  slug: amazon-sns-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-sns/refs/heads/main/openapi/amazon-sns-topics-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amazon Sns Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon SNS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon SNS
provider_slug: amazon-sns
slug: amazon-sns-domain-security
source_filename: amazon-sns-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-sns/refs/heads/main/security/amazon-sns-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email
- Messaging
- Notification
- Pub-Sub
- Push Notifications
- SMS
---
