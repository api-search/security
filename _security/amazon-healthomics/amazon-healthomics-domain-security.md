---
api_specs:
- filename: amazon-healthomics-annotationstore-api-openapi.yml
  format: yaml
  label: Amazon HealthOmics AnnotationStore API
  slug: amazon-healthomics-annotationstore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/openapi/amazon-healthomics-annotationstore-api-openapi.yml
- filename: amazon-healthomics-annotationstores-api-openapi.yml
  format: yaml
  label: Amazon HealthOmics AnnotationStores API
  slug: amazon-healthomics-annotationstores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/openapi/amazon-healthomics-annotationstores-api-openapi.yml
- filename: amazon-healthomics-import-api-openapi.yml
  format: yaml
  label: Amazon HealthOmics Import API
  slug: amazon-healthomics-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/openapi/amazon-healthomics-import-api-openapi.yml
- filename: amazon-healthomics-referencestore-api-openapi.yml
  format: yaml
  label: Amazon HealthOmics Referencestore API
  slug: amazon-healthomics-referencestore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/openapi/amazon-healthomics-referencestore-api-openapi.yml
- filename: amazon-healthomics-referencestores-api-openapi.yml
  format: yaml
  label: Amazon HealthOmics Referencestores API
  slug: amazon-healthomics-referencestores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/openapi/amazon-healthomics-referencestores-api-openapi.yml
- filename: amazon-healthomics-run-api-openapi.yml
  format: yaml
  label: Amazon HealthOmics Run API
  slug: amazon-healthomics-run-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/openapi/amazon-healthomics-run-api-openapi.yml
- filename: amazon-healthomics-rungroup-api-openapi.yml
  format: yaml
  label: Amazon HealthOmics RunGroup API
  slug: amazon-healthomics-rungroup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/openapi/amazon-healthomics-rungroup-api-openapi.yml
- filename: amazon-healthomics-sequencestore-api-openapi.yml
  format: yaml
  label: Amazon HealthOmics Sequencestore API
  slug: amazon-healthomics-sequencestore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/openapi/amazon-healthomics-sequencestore-api-openapi.yml
- filename: amazon-healthomics-sequencestores-api-openapi.yml
  format: yaml
  label: Amazon HealthOmics Sequencestores API
  slug: amazon-healthomics-sequencestores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/openapi/amazon-healthomics-sequencestores-api-openapi.yml
- filename: amazon-healthomics-tags-api-openapi.yml
  format: yaml
  label: Amazon HealthOmics Tags API
  slug: amazon-healthomics-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/openapi/amazon-healthomics-tags-api-openapi.yml
- filename: amazon-healthomics-variantstore-api-openapi.yml
  format: yaml
  label: Amazon HealthOmics VariantStore API
  slug: amazon-healthomics-variantstore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/openapi/amazon-healthomics-variantstore-api-openapi.yml
- filename: amazon-healthomics-variantstores-api-openapi.yml
  format: yaml
  label: Amazon HealthOmics VariantStores API
  slug: amazon-healthomics-variantstores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/openapi/amazon-healthomics-variantstores-api-openapi.yml
- filename: amazon-healthomics-workflow-api-openapi.yml
  format: yaml
  label: Amazon HealthOmics Workflow API
  slug: amazon-healthomics-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/openapi/amazon-healthomics-workflow-api-openapi.yml
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
- host: omics.amazonaws.com
  https: false
kind: domain-security
layout: security
method: probed
name: Amazon Healthomics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon HealthOmics, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
slug: amazon-healthomics-domain-security
source_filename: amazon-healthomics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: omics.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/security/amazon-healthomics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
---
