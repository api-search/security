---
api_specs:
- filename: amazon-iam-access-analyzer-access-preview-analyzerarn-api-openapi.yml
  format: yaml
  label: Amazon IAM Access Analyzer Access Preview#analyzerArn API
  slug: amazon-iam-access-analyzer-access-preview-analyzerarn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/openapi/amazon-iam-access-analyzer-access-preview-analyzerarn-api-openapi.yml
- filename: amazon-iam-access-analyzer-access-preview-api-openapi.yml
  format: yaml
  label: Amazon IAM Access Analyzer Access Preview API
  slug: amazon-iam-access-analyzer-access-preview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/openapi/amazon-iam-access-analyzer-access-preview-api-openapi.yml
- filename: amazon-iam-access-analyzer-analyzed-resource-analyzerarn-resourcearn-api-openapi.yml
  format: yaml
  label: Amazon IAM Access Analyzer Analyzed Resource#analyzerArn&resourceArn API
  slug: amazon-iam-access-analyzer-analyzed-resource-analyzerarn-resourcearn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/openapi/amazon-iam-access-analyzer-analyzed-resource-analyzerarn-resourcearn-api-openapi.yml
- filename: amazon-iam-access-analyzer-analyzed-resource-api-openapi.yml
  format: yaml
  label: Amazon IAM Access Analyzer Analyzed Resource API
  slug: amazon-iam-access-analyzer-analyzed-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/openapi/amazon-iam-access-analyzer-analyzed-resource-api-openapi.yml
- filename: amazon-iam-access-analyzer-analyzer-api-openapi.yml
  format: yaml
  label: Amazon IAM Access Analyzer Analyzer API
  slug: amazon-iam-access-analyzer-analyzer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/openapi/amazon-iam-access-analyzer-analyzer-api-openapi.yml
- filename: amazon-iam-access-analyzer-archive-rule-api-openapi.yml
  format: yaml
  label: Amazon IAM Access Analyzer Archive Rule API
  slug: amazon-iam-access-analyzer-archive-rule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/openapi/amazon-iam-access-analyzer-archive-rule-api-openapi.yml
- filename: amazon-iam-access-analyzer-finding-api-openapi.yml
  format: yaml
  label: Amazon IAM Access Analyzer Finding API
  slug: amazon-iam-access-analyzer-finding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/openapi/amazon-iam-access-analyzer-finding-api-openapi.yml
- filename: amazon-iam-access-analyzer-policy-api-openapi.yml
  format: yaml
  label: Amazon IAM Access Analyzer Policy API
  slug: amazon-iam-access-analyzer-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/openapi/amazon-iam-access-analyzer-policy-api-openapi.yml
- filename: amazon-iam-access-analyzer-resource-api-openapi.yml
  format: yaml
  label: Amazon IAM Access Analyzer Resource API
  slug: amazon-iam-access-analyzer-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/openapi/amazon-iam-access-analyzer-resource-api-openapi.yml
- filename: amazon-iam-access-analyzer-tags-api-openapi.yml
  format: yaml
  label: Amazon IAM Access Analyzer Tags API
  slug: amazon-iam-access-analyzer-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/openapi/amazon-iam-access-analyzer-tags-api-openapi.yml
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
- host: access-analyzer.amazonaws.com
  https: false
kind: domain-security
layout: security
method: probed
name: Amazon Iam Access Analyzer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon IAM Access Analyzer, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
slug: amazon-iam-access-analyzer-domain-security
source_filename: amazon-iam-access-analyzer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: access-analyzer.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/security/amazon-iam-access-analyzer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Access Control
- Compliance
- IAM
- Policy Management
- Security
---
