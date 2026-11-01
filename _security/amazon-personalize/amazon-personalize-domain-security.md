---
api_specs:
- filename: amazon-personalize-datasets-api-openapi.yml
  format: yaml
  label: Amazon Personalize Datasets API
  slug: amazon-personalize-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-personalize/openapi/amazon-personalize-datasets-api-openapi.yml
- filename: amazon-personalize-batch-inference-job-api-openapi.yml
  format: yaml
  label: Amazon Personalize Personalize Batch Inference Job API
  slug: amazon-personalize-batch-inference-job-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-personalize/openapi/amazon-personalize-batch-inference-job-api-openapi.yml
- filename: amazon-personalize-batch-segment-job-api-openapi.yml
  format: yaml
  label: Amazon Personalize Personalize Batch Segment Job API
  slug: amazon-personalize-batch-segment-job-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-personalize/openapi/amazon-personalize-batch-segment-job-api-openapi.yml
- filename: amazon-personalize-campaign-api-openapi.yml
  format: yaml
  label: Amazon Personalize Personalize Campaign API
  slug: amazon-personalize-campaign-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-personalize/openapi/amazon-personalize-campaign-api-openapi.yml
- filename: amazon-personalize-data-deletion-job-api-openapi.yml
  format: yaml
  label: Amazon Personalize Personalize Data Deletion Job API
  slug: amazon-personalize-data-deletion-job-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-personalize/openapi/amazon-personalize-data-deletion-job-api-openapi.yml
- filename: amazon-personalize-dataset-export-job-api-openapi.yml
  format: yaml
  label: Amazon Personalize Personalize Dataset Export Job API
  slug: amazon-personalize-dataset-export-job-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-personalize/openapi/amazon-personalize-dataset-export-job-api-openapi.yml
- filename: amazon-personalize-dataset-group-api-openapi.yml
  format: yaml
  label: Amazon Personalize Personalize Dataset Group API
  slug: amazon-personalize-dataset-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-personalize/openapi/amazon-personalize-dataset-group-api-openapi.yml
- filename: amazon-personalize-dataset-import-job-api-openapi.yml
  format: yaml
  label: Amazon Personalize Personalize Dataset Import Job API
  slug: amazon-personalize-dataset-import-job-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-personalize/openapi/amazon-personalize-dataset-import-job-api-openapi.yml
- filename: amazon-personalize-event-tracker-api-openapi.yml
  format: yaml
  label: Amazon Personalize Personalize Event Tracker API
  slug: amazon-personalize-event-tracker-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-personalize/openapi/amazon-personalize-event-tracker-api-openapi.yml
- filename: amazon-personalize-filter-api-openapi.yml
  format: yaml
  label: Amazon Personalize Personalize Filter API
  slug: amazon-personalize-filter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-personalize/openapi/amazon-personalize-filter-api-openapi.yml
- filename: amazon-personalize-metric-attribution-api-openapi.yml
  format: yaml
  label: Amazon Personalize Personalize Metric Attribution API
  slug: amazon-personalize-metric-attribution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-personalize/openapi/amazon-personalize-metric-attribution-api-openapi.yml
- filename: amazon-personalize-operations-api-openapi.yml
  format: yaml
  label: Amazon Personalize Personalize Operations API
  slug: amazon-personalize-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-personalize/openapi/amazon-personalize-operations-api-openapi.yml
- filename: amazon-personalize-recommender-api-openapi.yml
  format: yaml
  label: Amazon Personalize Personalize Recommender API
  slug: amazon-personalize-recommender-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-personalize/openapi/amazon-personalize-recommender-api-openapi.yml
- filename: amazon-personalize-schema-api-openapi.yml
  format: yaml
  label: Amazon Personalize Personalize Schema API
  slug: amazon-personalize-schema-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-personalize/openapi/amazon-personalize-schema-api-openapi.yml
- filename: amazon-personalize-solution-api-openapi.yml
  format: yaml
  label: Amazon Personalize Personalize Solution API
  slug: amazon-personalize-solution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-personalize/openapi/amazon-personalize-solution-api-openapi.yml
- filename: amazon-personalize-solution-version-api-openapi.yml
  format: yaml
  label: Amazon Personalize Personalize Solution Version API
  slug: amazon-personalize-solution-version-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-personalize/openapi/amazon-personalize-solution-version-api-openapi.yml
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
- host: personalize.amazonaws.com
  https: false
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Amazon Personalize Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Personalize, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Personalize
provider_slug: amazon-personalize
slug: amazon-personalize-domain-security
source_filename: amazon-personalize-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: personalize.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/amazon-personalize/security/amazon-personalize-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Customer Experience
- Machine Learning
- Personalization
- Recommendations
---
