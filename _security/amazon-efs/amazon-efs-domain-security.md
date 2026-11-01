---
api_specs:
- filename: amazon-efs-mount-targets-api-openapi.yml
  format: yaml
  label: Amazon EFS Mount Targets API
  slug: amazon-efs-mount-targets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-efs/openapi/amazon-efs-mount-targets-api-openapi.yml
- filename: amazon-efs-filesystems-api-openapi.yml
  format: yaml
  label: Amazon EFS Filesystems API
  slug: amazon-efs-filesystems-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-efs/openapi/amazon-efs-filesystems-api-openapi.yml
- filename: amazon-efs-access-points-api-openapi.yml
  format: yaml
  label: Amazon EFS Efs Access Points API
  slug: amazon-efs-access-points-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-efs/openapi/amazon-efs-access-points-api-openapi.yml
- filename: amazon-efs-operations-api-openapi.yml
  format: yaml
  label: Amazon EFS Efs Operations API
  slug: amazon-efs-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-efs/openapi/amazon-efs-operations-api-openapi.yml
- filename: amazon-efs-policy-api-openapi.yml
  format: yaml
  label: Amazon EFS Efs Policy API
  slug: amazon-efs-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-efs/openapi/amazon-efs-policy-api-openapi.yml
- filename: amazon-efs-resource-tags-api-openapi.yml
  format: yaml
  label: Amazon EFS Efs Resource Tags API
  slug: amazon-efs-resource-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-efs/openapi/amazon-efs-resource-tags-api-openapi.yml
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
- host: elasticfilesystem.amazonaws.com
  https: false
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Amazon Efs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon EFS, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon EFS
provider_slug: amazon-efs
slug: amazon-efs-domain-security
source_filename: amazon-efs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: elasticfilesystem.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/amazon-efs/security/amazon-efs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Amazon Web Services
- EFS
- Elastic File System
- File Storage
- NFS
- Serverless
- Storage
---
