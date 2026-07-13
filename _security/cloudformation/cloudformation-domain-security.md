---
api_specs:
- filename: cloudformation-api.yml
  format: yaml
  label: AWS CloudFormation API
  slug: aws-cloudformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/openapi/cloudformation-api.yml
- filename: cloud-control-api.yml
  format: yaml
  label: AWS Cloud Control API
  slug: aws-cloud-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/openapi/cloud-control-api.yml
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
