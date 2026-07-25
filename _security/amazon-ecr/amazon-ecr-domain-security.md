---
api_specs:
- filename: amazon-ecr-amazon-ecr-amazon-elastic-container-registry-ecr-api-api-openapi.yml
  format: yaml
  label: Amazon ECR Amazon ECR Amazon Elastic Container Registry (ECR) API API
  slug: amazon-ecr-amazon-ecr-amazon-elastic-container-registry-ecr-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ecr/refs/heads/main/openapi/amazon-ecr-amazon-ecr-amazon-elastic-container-registry-ecr-api-api-openapi.yml
- filename: amazon-ecr-batchgetimage-api-openapi.yml
  format: yaml
  label: 'Amazon ECR #BatchGetImage API'
  slug: amazon-ecr-batchgetimage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ecr/refs/heads/main/openapi/amazon-ecr-batchgetimage-api-openapi.yml
- filename: amazon-ecr-deleterepository-api-openapi.yml
  format: yaml
  label: 'Amazon ECR #DeleteRepository API'
  slug: amazon-ecr-deleterepository-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ecr/refs/heads/main/openapi/amazon-ecr-deleterepository-api-openapi.yml
- filename: amazon-ecr-describerepositories-api-openapi.yml
  format: yaml
  label: 'Amazon ECR #DescribeRepositories API'
  slug: amazon-ecr-describerepositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ecr/refs/heads/main/openapi/amazon-ecr-describerepositories-api-openapi.yml
- filename: amazon-ecr-listimages-api-openapi.yml
  format: yaml
  label: 'Amazon ECR #ListImages API'
  slug: amazon-ecr-listimages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ecr/refs/heads/main/openapi/amazon-ecr-listimages-api-openapi.yml
- filename: amazon-ecr-putimage-api-openapi.yml
  format: yaml
  label: 'Amazon ECR #PutImage API'
  slug: amazon-ecr-putimage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ecr/refs/heads/main/openapi/amazon-ecr-putimage-api-openapi.yml
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
- host: api.ecr.amazonaws.com
  https: false
kind: domain-security
layout: security
method: probed
name: Amazon Ecr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon ECR, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon ECR
provider_slug: amazon-ecr
slug: amazon-ecr-domain-security
source_filename: amazon-ecr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: api.ecr.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecr/refs/heads/main/security/amazon-ecr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Amazon Web Services
- Container Images
- Container Registry
- Containers
- Docker
- ECR
- OCI
---
