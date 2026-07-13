---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Amazon ECS API (Fargate)
  slug: amazon-ecs-api-fargate
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/ecs/2014-11-13/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Amazon EKS API (Fargate)
  slug: amazon-eks-api-fargate
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/eks/2017-11-01/openapi.yaml
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
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: docs.aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fargate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AWS Fargate, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AWS Fargate
provider_slug: fargate
slug: fargate-domain-security
source_filename: fargate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: docs.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fargate/refs/heads/main/security/fargate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Compute
- Containers
- Docker
- Kubernetes
- Serverless
---
