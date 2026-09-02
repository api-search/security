---
api_specs:
- filename: amazon-ecs-capacity-providers-api-openapi.yml
  format: yaml
  label: Amazon ECS Capacity Providers API
  slug: amazon-ecs-capacity-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/openapi/amazon-ecs-capacity-providers-api-openapi.yml
- filename: amazon-ecs-clusters-api-openapi.yml
  format: yaml
  label: Amazon ECS Clusters API
  slug: amazon-ecs-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/openapi/amazon-ecs-clusters-api-openapi.yml
- filename: amazon-ecs-container-instances-api-openapi.yml
  format: yaml
  label: Amazon ECS Container Instances API
  slug: amazon-ecs-container-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/openapi/amazon-ecs-container-instances-api-openapi.yml
- filename: amazon-ecs-task-definitions-api-openapi.yml
  format: yaml
  label: Amazon ECS Task Definitions API
  slug: amazon-ecs-task-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/openapi/amazon-ecs-task-definitions-api-openapi.yml
- filename: amazon-ecs-tasks-api-openapi.yml
  format: yaml
  label: Amazon ECS Tasks API
  slug: amazon-ecs-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/openapi/amazon-ecs-tasks-api-openapi.yml
- filename: amazon-ecs-x-amz-target-amazonec2containerservicev20141113-createservice-api-openapi.yml
  format: yaml
  label: 'Amazon ECS #X Amz Target=AmazonEC2ContainerServiceV20141113.CreateService API'
  slug: amazon-ecs-x-amz-target-amazonec2containerservicev20141113-createservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/openapi/amazon-ecs-x-amz-target-amazonec2containerservicev20141113-createservice-api-openapi.yml
- filename: amazon-ecs-x-amz-target-amazonec2containerservicev20141113-deleteservice-api-openapi.yml
  format: yaml
  label: 'Amazon ECS #X Amz Target=AmazonEC2ContainerServiceV20141113.DeleteService API'
  slug: amazon-ecs-x-amz-target-amazonec2containerservicev20141113-deleteservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/openapi/amazon-ecs-x-amz-target-amazonec2containerservicev20141113-deleteservice-api-openapi.yml
- filename: amazon-ecs-x-amz-target-amazonec2containerservicev20141113-describeservices-api-openapi.yml
  format: yaml
  label: 'Amazon ECS #X Amz Target=AmazonEC2ContainerServiceV20141113.DescribeServices API'
  slug: amazon-ecs-x-amz-target-amazonec2containerservicev20141113-describeservices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/openapi/amazon-ecs-x-amz-target-amazonec2containerservicev20141113-describeservices-api-openapi.yml
- filename: amazon-ecs-x-amz-target-amazonec2containerservicev20141113-listservices-api-openapi.yml
  format: yaml
  label: 'Amazon ECS #X Amz Target=AmazonEC2ContainerServiceV20141113.ListServices API'
  slug: amazon-ecs-x-amz-target-amazonec2containerservicev20141113-listservices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/openapi/amazon-ecs-x-amz-target-amazonec2containerservicev20141113-listservices-api-openapi.yml
- filename: amazon-ecs-x-amz-target-amazonec2containerservicev20141113-updateservice-api-openapi.yml
  format: yaml
  label: 'Amazon ECS #X Amz Target=AmazonEC2ContainerServiceV20141113.UpdateService API'
  slug: amazon-ecs-x-amz-target-amazonec2containerservicev20141113-updateservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/openapi/amazon-ecs-x-amz-target-amazonec2containerservicev20141113-updateservice-api-openapi.yml
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
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/security/amazon-ecs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Amazon
- Containers
- Docker
- ECS
- Orchestration
---
