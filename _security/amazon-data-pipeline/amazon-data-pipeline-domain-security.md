---
api_specs:
- filename: amazon-data-pipeline-pipeline-objects-api-openapi.yml
  format: yaml
  label: Amazon Data Pipeline Pipeline Objects API
  slug: amazon-data-pipeline-pipeline-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-data-pipeline/refs/heads/main/openapi/amazon-data-pipeline-pipeline-objects-api-openapi.yml
- filename: amazon-data-pipeline-pipeline-runs-api-openapi.yml
  format: yaml
  label: Amazon Data Pipeline Pipeline Runs API
  slug: amazon-data-pipeline-pipeline-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-data-pipeline/refs/heads/main/openapi/amazon-data-pipeline-pipeline-runs-api-openapi.yml
- filename: amazon-data-pipeline-pipelines-api-openapi.yml
  format: yaml
  label: Amazon Data Pipeline Pipelines API
  slug: amazon-data-pipeline-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-data-pipeline/refs/heads/main/openapi/amazon-data-pipeline-pipelines-api-openapi.yml
- filename: amazon-data-pipeline-tags-api-openapi.yml
  format: yaml
  label: Amazon Data Pipeline Tags API
  slug: amazon-data-pipeline-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-data-pipeline/refs/heads/main/openapi/amazon-data-pipeline-tags-api-openapi.yml
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
- host: datapipeline.amazonaws.com
  https: false
kind: domain-security
layout: security
method: probed
name: Amazon Data Pipeline Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Data Pipeline, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Data Pipeline
provider_slug: amazon-data-pipeline
slug: amazon-data-pipeline-domain-security
source_filename: amazon-data-pipeline-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: datapipeline.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-pipeline/refs/heads/main/security/amazon-data-pipeline-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Processing
- ETL
- Workflows
- Data Pipeline
- Automation
---
