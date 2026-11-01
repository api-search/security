---
api_specs:
- filename: amazon-elasticache-amazon-elasticache-api-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Amazon ElastiCache API
  slug: amazon-elasticache-amazon-elasticache-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-amazon-elasticache-api-api-openapi.yml
- filename: amazon-elasticache-cache-parameter-group-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache Cache Parameter Group API
  slug: amazon-elasticache-cache-parameter-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-cache-parameter-group-api-openapi.yml
- filename: amazon-elasticache-cache-security-group-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache Cache Security Group API
  slug: amazon-elasticache-cache-security-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-cache-security-group-api-openapi.yml
- filename: amazon-elasticache-cache-subnet-group-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache Cache Subnet Group API
  slug: amazon-elasticache-cache-subnet-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-cache-subnet-group-api-openapi.yml
- filename: amazon-elasticache-global-replication-group-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache Global Replication Group API
  slug: amazon-elasticache-global-replication-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-global-replication-group-api-openapi.yml
- filename: amazon-elasticache-migration-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache Migration API
  slug: amazon-elasticache-migration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-migration-api-openapi.yml
- filename: amazon-elasticache-operations-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache Operations API
  slug: amazon-elasticache-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-operations-api-openapi.yml
- filename: amazon-elasticache-serverless-cache-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache Serverless Cache API
  slug: amazon-elasticache-serverless-cache-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-serverless-cache-api-openapi.yml
- filename: amazon-elasticache-serverless-cache-snapshot-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache Serverless Cache Snapshot API
  slug: amazon-elasticache-serverless-cache-snapshot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-serverless-cache-snapshot-api-openapi.yml
- filename: amazon-elasticache-snapshot-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache Snapshot API
  slug: amazon-elasticache-snapshot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-snapshot-api-openapi.yml
- filename: amazon-elasticache-tag-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache Tag API
  slug: amazon-elasticache-tag-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-tag-api-openapi.yml
- filename: amazon-elasticache-update-action-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache Update Action API
  slug: amazon-elasticache-update-action-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-update-action-api-openapi.yml
- filename: amazon-elasticache-user-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache User API
  slug: amazon-elasticache-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-user-api-openapi.yml
- filename: amazon-elasticache-user-group-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache User Group API
  slug: amazon-elasticache-user-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-user-group-api-openapi.yml
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
- host: elasticache.amazonaws.com
  https: false
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Amazon Elasticache Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon ElastiCache, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon ElastiCache
provider_slug: amazon-elasticache
slug: amazon-elasticache-domain-security
source_filename: amazon-elasticache-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: elasticache.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/amazon-elasticache/security/amazon-elasticache-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Amazon Web Services
- Caching
- Database
- ElastiCache
- In-Memory
- Memcached
- Redis
---
