---
api_specs:
- filename: amazon-ecs-capacity-providers-api-openapi.yml
  format: yaml
  label: Amazon ECS Capacity Providers API
  slug: amazon-ecs-capacity-providers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ecs/openapi/amazon-ecs-capacity-providers-api-openapi.yml
- filename: amazon-ecs-clusters-api-openapi.yml
  format: yaml
  label: Amazon ECS Clusters API
  slug: amazon-ecs-clusters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ecs/openapi/amazon-ecs-clusters-api-openapi.yml
- filename: amazon-ecs-container-instances-api-openapi.yml
  format: yaml
  label: Amazon ECS Container Instances API
  slug: amazon-ecs-container-instances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ecs/openapi/amazon-ecs-container-instances-api-openapi.yml
- filename: amazon-ecs-task-definitions-api-openapi.yml
  format: yaml
  label: Amazon ECS Task Definitions API
  slug: amazon-ecs-task-definitions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ecs/openapi/amazon-ecs-task-definitions-api-openapi.yml
- filename: amazon-ecs-tasks-api-openapi.yml
  format: yaml
  label: Amazon ECS Tasks API
  slug: amazon-ecs-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ecs/openapi/amazon-ecs-tasks-api-openapi.yml
- filename: amazon-ecs-amazon-ecs-amazon-elastic-container-service-ecs-api-api-openapi.yml
  format: yaml
  label: Amazon ECS Amazon ECS Amazon Elastic Container Service (ECS) API
  slug: amazon-ecs-amazon-ecs-amazon-elastic-container-service-ecs-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ecs/openapi/amazon-ecs-amazon-ecs-amazon-elastic-container-service-ecs-api-api-openapi.yml
- filename: amazon-ecs-account-setting-api-openapi.yml
  format: yaml
  label: Amazon ECS Ecs Account Setting API
  slug: amazon-ecs-account-setting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ecs/openapi/amazon-ecs-account-setting-api-openapi.yml
- filename: amazon-ecs-attribute-api-openapi.yml
  format: yaml
  label: Amazon ECS Ecs Attribute API
  slug: amazon-ecs-attribute-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ecs/openapi/amazon-ecs-attribute-api-openapi.yml
- filename: amazon-ecs-daemon-api-openapi.yml
  format: yaml
  label: Amazon ECS Ecs Daemon API
  slug: amazon-ecs-daemon-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ecs/openapi/amazon-ecs-daemon-api-openapi.yml
- filename: amazon-ecs-daemon-task-definition-api-openapi.yml
  format: yaml
  label: Amazon ECS Ecs Daemon Task Definition API
  slug: amazon-ecs-daemon-task-definition-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ecs/openapi/amazon-ecs-daemon-task-definition-api-openapi.yml
- filename: amazon-ecs-express-gateway-service-api-openapi.yml
  format: yaml
  label: Amazon ECS Ecs Express Gateway Service API
  slug: amazon-ecs-express-gateway-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ecs/openapi/amazon-ecs-express-gateway-service-api-openapi.yml
- filename: amazon-ecs-gateway-api-openapi.yml
  format: yaml
  label: Amazon ECS Ecs Gateway API
  slug: amazon-ecs-gateway-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ecs/openapi/amazon-ecs-gateway-api-openapi.yml
- filename: amazon-ecs-operations-api-openapi.yml
  format: yaml
  label: Amazon ECS Ecs Operations API
  slug: amazon-ecs-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ecs/openapi/amazon-ecs-operations-api-openapi.yml
- filename: amazon-ecs-service-deployment-api-openapi.yml
  format: yaml
  label: Amazon ECS Ecs Service Deployment API
  slug: amazon-ecs-service-deployment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ecs/openapi/amazon-ecs-service-deployment-api-openapi.yml
- filename: amazon-ecs-task-set-api-openapi.yml
  format: yaml
  label: Amazon ECS Ecs Task Set API
  slug: amazon-ecs-task-set-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ecs/openapi/amazon-ecs-task-set-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazonaws.com
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- host: ecs.amazonaws.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''ecs.amazona'
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: docs.aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Amazon Ecs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon ECS, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon ECS
provider_slug: amazon-ecs
slug: amazon-ecs-domain-security
source_filename: amazon-ecs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: ecs.amazonaws.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''ecs.amazona'\n  hsts: null\n- host: docs.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/amazon-ecs/security/amazon-ecs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Amazon
- Containers
- Docker
- ECS
- Container Orchestration
---
