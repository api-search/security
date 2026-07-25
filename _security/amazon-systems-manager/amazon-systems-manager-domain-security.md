---
api_specs:
- filename: amazon-systems-manager-automation-api-openapi.yml
  format: yaml
  label: Amazon Systems Manager Automation API
  slug: amazon-systems-manager-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-systems-manager/refs/heads/main/openapi/amazon-systems-manager-automation-api-openapi.yml
- filename: amazon-systems-manager-documents-api-openapi.yml
  format: yaml
  label: Amazon Systems Manager Documents API
  slug: amazon-systems-manager-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-systems-manager/refs/heads/main/openapi/amazon-systems-manager-documents-api-openapi.yml
- filename: amazon-systems-manager-managed-instances-api-openapi.yml
  format: yaml
  label: Amazon Systems Manager Managed Instances API
  slug: amazon-systems-manager-managed-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-systems-manager/refs/heads/main/openapi/amazon-systems-manager-managed-instances-api-openapi.yml
- filename: amazon-systems-manager-parameter-store-api-openapi.yml
  format: yaml
  label: Amazon Systems Manager Parameter Store API
  slug: amazon-systems-manager-parameter-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-systems-manager/refs/heads/main/openapi/amazon-systems-manager-parameter-store-api-openapi.yml
- filename: amazon-systems-manager-run-command-api-openapi.yml
  format: yaml
  label: Amazon Systems Manager Run Command API
  slug: amazon-systems-manager-run-command-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-systems-manager/refs/heads/main/openapi/amazon-systems-manager-run-command-api-openapi.yml
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
- host: ssm.amazonaws.com
  https: false
kind: domain-security
layout: security
method: probed
name: Amazon Systems Manager Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Systems Manager, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Systems Manager
provider_slug: amazon-systems-manager
slug: amazon-systems-manager-domain-security
source_filename: amazon-systems-manager-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: ssm.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-systems-manager/refs/heads/main/security/amazon-systems-manager-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automation
- Management
- Operations
---
