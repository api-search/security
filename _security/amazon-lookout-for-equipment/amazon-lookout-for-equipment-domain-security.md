---
api_specs:
- filename: amazon-lookout-for-equipment-datasets-api-openapi.yml
  format: yaml
  label: Amazon Lookout for Equipment Datasets API
  slug: amazon-lookout-for-equipment-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-lookout-for-equipment/openapi/amazon-lookout-for-equipment-datasets-api-openapi.yml
- filename: amazon-lookout-for-equipment-data-ingestion-job-api-openapi.yml
  format: yaml
  label: Amazon Lookout for Equipment Lookout For Equipment Data Ingestion Job API
  slug: amazon-lookout-for-equipment-data-ingestion-job-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-lookout-for-equipment/openapi/amazon-lookout-for-equipment-data-ingestion-job-api-openapi.yml
- filename: amazon-lookout-for-equipment-inference-scheduler-api-openapi.yml
  format: yaml
  label: Amazon Lookout for Equipment Lookout For Equipment Inference Scheduler API
  slug: amazon-lookout-for-equipment-inference-scheduler-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-lookout-for-equipment/openapi/amazon-lookout-for-equipment-inference-scheduler-api-openapi.yml
- filename: amazon-lookout-for-equipment-label-api-openapi.yml
  format: yaml
  label: Amazon Lookout for Equipment Lookout For Equipment Label API
  slug: amazon-lookout-for-equipment-label-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-lookout-for-equipment/openapi/amazon-lookout-for-equipment-label-api-openapi.yml
- filename: amazon-lookout-for-equipment-label-group-api-openapi.yml
  format: yaml
  label: Amazon Lookout for Equipment Lookout For Equipment Label Group API
  slug: amazon-lookout-for-equipment-label-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-lookout-for-equipment/openapi/amazon-lookout-for-equipment-label-group-api-openapi.yml
- filename: amazon-lookout-for-equipment-model-version-api-openapi.yml
  format: yaml
  label: Amazon Lookout for Equipment Lookout For Equipment Model Version API
  slug: amazon-lookout-for-equipment-model-version-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-lookout-for-equipment/openapi/amazon-lookout-for-equipment-model-version-api-openapi.yml
- filename: amazon-lookout-for-equipment-operations-api-openapi.yml
  format: yaml
  label: Amazon Lookout for Equipment Lookout For Equipment Operations API
  slug: amazon-lookout-for-equipment-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-lookout-for-equipment/openapi/amazon-lookout-for-equipment-operations-api-openapi.yml
- filename: amazon-lookout-for-equipment-resource-policy-api-openapi.yml
  format: yaml
  label: Amazon Lookout for Equipment Lookout For Equipment Resource Policy API
  slug: amazon-lookout-for-equipment-resource-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-lookout-for-equipment/openapi/amazon-lookout-for-equipment-resource-policy-api-openapi.yml
- filename: amazon-lookout-for-equipment-retraining-scheduler-api-openapi.yml
  format: yaml
  label: Amazon Lookout for Equipment Lookout For Equipment Retraining Scheduler API
  slug: amazon-lookout-for-equipment-retraining-scheduler-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-lookout-for-equipment/openapi/amazon-lookout-for-equipment-retraining-scheduler-api-openapi.yml
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
- host: lookoutequipment.amazonaws.com
  https: false
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: lookoutequipment.us-east-1.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Amazon Lookout For Equipment Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Lookout for Equipment, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Lookout for Equipment
provider_slug: amazon-lookout-for-equipment
slug: amazon-lookout-for-equipment-domain-security
source_filename: amazon-lookout-for-equipment-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: lookoutequipment.amazonaws.com\n  https: false\n- host: lookoutequipment.us-east-1.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/amazon-lookout-for-equipment/security/amazon-lookout-for-equipment-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Equipment Monitoring
- Industrial IoT
- Machine Learning
- Predictive Maintenance
---
