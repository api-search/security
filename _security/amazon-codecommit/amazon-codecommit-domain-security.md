---
api_specs:
- filename: amazon-codecommit-approval-rule-template-api-openapi.yml
  format: yaml
  label: Amazon CodeCommit Codecommit Approval Rule Template API
  slug: amazon-codecommit-approval-rule-template-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-codecommit/openapi/amazon-codecommit-approval-rule-template-api-openapi.yml
- filename: amazon-codecommit-branch-api-openapi.yml
  format: yaml
  label: Amazon CodeCommit Codecommit Branch API
  slug: amazon-codecommit-branch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-codecommit/openapi/amazon-codecommit-branch-api-openapi.yml
- filename: amazon-codecommit-comment-api-openapi.yml
  format: yaml
  label: Amazon CodeCommit Codecommit Comment API
  slug: amazon-codecommit-comment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-codecommit/openapi/amazon-codecommit-comment-api-openapi.yml
- filename: amazon-codecommit-commit-api-openapi.yml
  format: yaml
  label: Amazon CodeCommit Codecommit Commit API
  slug: amazon-codecommit-commit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-codecommit/openapi/amazon-codecommit-commit-api-openapi.yml
- filename: amazon-codecommit-file-api-openapi.yml
  format: yaml
  label: Amazon CodeCommit Codecommit File API
  slug: amazon-codecommit-file-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-codecommit/openapi/amazon-codecommit-file-api-openapi.yml
- filename: amazon-codecommit-merge-conflict-api-openapi.yml
  format: yaml
  label: Amazon CodeCommit Codecommit Merge Conflict API
  slug: amazon-codecommit-merge-conflict-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-codecommit/openapi/amazon-codecommit-merge-conflict-api-openapi.yml
- filename: amazon-codecommit-operations-api-openapi.yml
  format: yaml
  label: Amazon CodeCommit Codecommit Operations API
  slug: amazon-codecommit-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-codecommit/openapi/amazon-codecommit-operations-api-openapi.yml
- filename: amazon-codecommit-pull-request-api-openapi.yml
  format: yaml
  label: Amazon CodeCommit Codecommit Pull Request API
  slug: amazon-codecommit-pull-request-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-codecommit/openapi/amazon-codecommit-pull-request-api-openapi.yml
- filename: amazon-codecommit-repository-api-openapi.yml
  format: yaml
  label: Amazon CodeCommit Codecommit Repository API
  slug: amazon-codecommit-repository-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-codecommit/openapi/amazon-codecommit-repository-api-openapi.yml
- filename: amazon-codecommit-repository-trigger-api-openapi.yml
  format: yaml
  label: Amazon CodeCommit Codecommit Repository Trigger API
  slug: amazon-codecommit-repository-trigger-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-codecommit/openapi/amazon-codecommit-repository-trigger-api-openapi.yml
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
name: Amazon Codecommit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon CodeCommit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon CodeCommit
provider_slug: amazon-codecommit
slug: amazon-codecommit-domain-security
source_filename: amazon-codecommit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 47304000\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/amazon-codecommit/security/amazon-codecommit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Version Control
- Cloud
---
