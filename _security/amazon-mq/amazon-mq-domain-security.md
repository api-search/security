---
api_specs:
- filename: amazon-mq-broker-engine-types-api-openapi.yml
  format: yaml
  label: Amazon MQ Broker Engine Types API
  slug: amazon-mq-broker-engine-types-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-mq/openapi/amazon-mq-broker-engine-types-api-openapi.yml
- filename: amazon-mq-broker-instance-options-api-openapi.yml
  format: yaml
  label: Amazon MQ Broker Instance Options API
  slug: amazon-mq-broker-instance-options-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-mq/openapi/amazon-mq-broker-instance-options-api-openapi.yml
- filename: amazon-mq-brokers-api-openapi.yml
  format: yaml
  label: Amazon MQ Brokers API
  slug: amazon-mq-brokers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-mq/openapi/amazon-mq-brokers-api-openapi.yml
- filename: amazon-mq-configurations-api-openapi.yml
  format: yaml
  label: Amazon MQ Configurations API
  slug: amazon-mq-configurations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-mq/openapi/amazon-mq-configurations-api-openapi.yml
- filename: amazon-mq-tags-api-openapi.yml
  format: yaml
  label: Amazon MQ Tags API
  slug: amazon-mq-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-mq/openapi/amazon-mq-tags-api-openapi.yml
- filename: amazon-mq-operations-api-openapi.yml
  format: yaml
  label: Amazon MQ Mq Operations API
  slug: amazon-mq-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-mq/openapi/amazon-mq-operations-api-openapi.yml
- filename: amazon-mq-users-api-openapi.yml
  format: yaml
  label: Amazon MQ Mq Users API
  slug: amazon-mq-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-mq/openapi/amazon-mq-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
hosts:
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Amazon MQ Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon MQ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon MQ
provider_slug: amazon-mq
slug: amazon-mq-domain-security
source_filename: amazon-mq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 47304000\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/amazon-mq/security/amazon-mq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Amazon Web Services
- Message Queue
- Messaging
- Message Broker
- RabbitMQ
---
