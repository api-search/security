---
api_specs:
- filename: cloudformation-change-sets-api-openapi.yml
  format: yaml
  label: AWS CloudFormation Change Sets API
  slug: cloudformation-change-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/openapi/cloudformation-change-sets-api-openapi.yml
- filename: cloudformation-exports-api-openapi.yml
  format: yaml
  label: AWS CloudFormation Exports API
  slug: cloudformation-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/openapi/cloudformation-exports-api-openapi.yml
- filename: cloudformation-registry-api-openapi.yml
  format: yaml
  label: AWS CloudFormation Registry API
  slug: cloudformation-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/openapi/cloudformation-registry-api-openapi.yml
- filename: cloudformation-request-status-api-openapi.yml
  format: yaml
  label: AWS CloudFormation Request Status API
  slug: cloudformation-request-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/openapi/cloudformation-request-status-api-openapi.yml
- filename: cloudformation-resources-api-openapi.yml
  format: yaml
  label: AWS CloudFormation Resources API
  slug: cloudformation-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/openapi/cloudformation-resources-api-openapi.yml
- filename: cloudformation-stack-drift-api-openapi.yml
  format: yaml
  label: AWS CloudFormation Stack Drift API
  slug: cloudformation-stack-drift-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/openapi/cloudformation-stack-drift-api-openapi.yml
- filename: cloudformation-stack-events-api-openapi.yml
  format: yaml
  label: AWS CloudFormation Stack Events API
  slug: cloudformation-stack-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/openapi/cloudformation-stack-events-api-openapi.yml
- filename: cloudformation-stack-instances-api-openapi.yml
  format: yaml
  label: AWS CloudFormation Stack Instances API
  slug: cloudformation-stack-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/openapi/cloudformation-stack-instances-api-openapi.yml
- filename: cloudformation-stack-policies-api-openapi.yml
  format: yaml
  label: AWS CloudFormation Stack Policies API
  slug: cloudformation-stack-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/openapi/cloudformation-stack-policies-api-openapi.yml
- filename: cloudformation-stack-resources-api-openapi.yml
  format: yaml
  label: AWS CloudFormation Stack Resources API
  slug: cloudformation-stack-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/openapi/cloudformation-stack-resources-api-openapi.yml
- filename: cloudformation-stack-sets-api-openapi.yml
  format: yaml
  label: AWS CloudFormation Stack Sets API
  slug: cloudformation-stack-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/openapi/cloudformation-stack-sets-api-openapi.yml
- filename: cloudformation-stacks-api-openapi.yml
  format: yaml
  label: AWS CloudFormation Stacks API
  slug: cloudformation-stacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/openapi/cloudformation-stacks-api-openapi.yml
- filename: cloudformation-templates-api-openapi.yml
  format: yaml
  label: AWS CloudFormation Templates API
  slug: cloudformation-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/openapi/cloudformation-templates-api-openapi.yml
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
kind: domain-security
layout: security
method: probed
name: Cloudformation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AWS CloudFormation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AWS CloudFormation
provider_slug: cloudformation
slug: cloudformation-domain-security
source_filename: cloudformation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/security/cloudformation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automation
- Cloud Resources
- IaC
- Infrastructure As Code
- Stack Management
---
