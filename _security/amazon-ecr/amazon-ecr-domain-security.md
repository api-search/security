---
api_specs:
- filename: amazon-ecr-amazon-ecr-amazon-elastic-container-registry-ecr-api-api-openapi.yml
  format: yaml
  label: Amazon ECR Amazon ECR Amazon Elastic Container Registry (ECR) API
  slug: amazon-ecr-amazon-ecr-amazon-elastic-container-registry-ecr-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ecr/openapi/amazon-ecr-amazon-ecr-amazon-elastic-container-registry-ecr-api-api-openapi.yml
- filename: amazon-ecr-lifecycle-policy-api-openapi.yml
  format: yaml
  label: Amazon ECR Ecr Lifecycle Policy API
  slug: amazon-ecr-lifecycle-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ecr/openapi/amazon-ecr-lifecycle-policy-api-openapi.yml
- filename: amazon-ecr-operations-api-openapi.yml
  format: yaml
  label: Amazon ECR Ecr Operations API
  slug: amazon-ecr-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ecr/openapi/amazon-ecr-operations-api-openapi.yml
- filename: amazon-ecr-pull-through-cache-rule-api-openapi.yml
  format: yaml
  label: Amazon ECR Ecr Pull Through Cache Rule API
  slug: amazon-ecr-pull-through-cache-rule-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ecr/openapi/amazon-ecr-pull-through-cache-rule-api-openapi.yml
- filename: amazon-ecr-pull-time-update-exclusion-api-openapi.yml
  format: yaml
  label: Amazon ECR Ecr Pull Time Update Exclusion API
  slug: amazon-ecr-pull-time-update-exclusion-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ecr/openapi/amazon-ecr-pull-time-update-exclusion-api-openapi.yml
- filename: amazon-ecr-registry-policy-api-openapi.yml
  format: yaml
  label: Amazon ECR Ecr Registry Policy API
  slug: amazon-ecr-registry-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ecr/openapi/amazon-ecr-registry-policy-api-openapi.yml
- filename: amazon-ecr-replication-backfill-api-openapi.yml
  format: yaml
  label: Amazon ECR Ecr Replication Backfill API
  slug: amazon-ecr-replication-backfill-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ecr/openapi/amazon-ecr-replication-backfill-api-openapi.yml
- filename: amazon-ecr-repository-creation-template-api-openapi.yml
  format: yaml
  label: Amazon ECR Ecr Repository Creation Template API
  slug: amazon-ecr-repository-creation-template-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ecr/openapi/amazon-ecr-repository-creation-template-api-openapi.yml
- filename: amazon-ecr-repository-policy-api-openapi.yml
  format: yaml
  label: Amazon ECR Ecr Repository Policy API
  slug: amazon-ecr-repository-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ecr/openapi/amazon-ecr-repository-policy-api-openapi.yml
- filename: amazon-ecr-signing-configuration-api-openapi.yml
  format: yaml
  label: Amazon ECR Ecr Signing Configuration API
  slug: amazon-ecr-signing-configuration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ecr/openapi/amazon-ecr-signing-configuration-api-openapi.yml
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
hosts_probed: 2
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
source_yaml_url: https://artifacts.apis.io/amazon-ecr/security/amazon-ecr-domain-security.yml
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
