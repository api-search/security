---
api_specs:
- filename: amazon-transcribe-transcription-jobs-api-openapi.yml
  format: yaml
  label: Amazon Transcribe Transcription Jobs API
  slug: amazon-transcribe-transcription-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-transcribe/openapi/amazon-transcribe-transcription-jobs-api-openapi.yml
- filename: amazon-transcribe-vocabularies-api-openapi.yml
  format: yaml
  label: Amazon Transcribe Vocabularies API
  slug: amazon-transcribe-vocabularies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-transcribe/openapi/amazon-transcribe-vocabularies-api-openapi.yml
- filename: amazon-transcribe-call-analytics-category-api-openapi.yml
  format: yaml
  label: Amazon Transcribe Transcribe Call Analytics Category API
  slug: amazon-transcribe-call-analytics-category-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-transcribe/openapi/amazon-transcribe-call-analytics-category-api-openapi.yml
- filename: amazon-transcribe-call-analytics-job-api-openapi.yml
  format: yaml
  label: Amazon Transcribe Transcribe Call Analytics Job API
  slug: amazon-transcribe-call-analytics-job-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-transcribe/openapi/amazon-transcribe-call-analytics-job-api-openapi.yml
- filename: amazon-transcribe-language-model-api-openapi.yml
  format: yaml
  label: Amazon Transcribe Transcribe Language Model API
  slug: amazon-transcribe-language-model-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-transcribe/openapi/amazon-transcribe-language-model-api-openapi.yml
- filename: amazon-transcribe-medical-scribe-job-api-openapi.yml
  format: yaml
  label: Amazon Transcribe Transcribe Medical Scribe Job API
  slug: amazon-transcribe-medical-scribe-job-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-transcribe/openapi/amazon-transcribe-medical-scribe-job-api-openapi.yml
- filename: amazon-transcribe-medical-transcription-job-api-openapi.yml
  format: yaml
  label: Amazon Transcribe Transcribe Medical Transcription Job API
  slug: amazon-transcribe-medical-transcription-job-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-transcribe/openapi/amazon-transcribe-medical-transcription-job-api-openapi.yml
- filename: amazon-transcribe-medical-vocabulary-api-openapi.yml
  format: yaml
  label: Amazon Transcribe Transcribe Medical Vocabulary API
  slug: amazon-transcribe-medical-vocabulary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-transcribe/openapi/amazon-transcribe-medical-vocabulary-api-openapi.yml
- filename: amazon-transcribe-operations-api-openapi.yml
  format: yaml
  label: Amazon Transcribe Transcribe Operations API
  slug: amazon-transcribe-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-transcribe/openapi/amazon-transcribe-operations-api-openapi.yml
- filename: amazon-transcribe-vocabulary-filter-api-openapi.yml
  format: yaml
  label: Amazon Transcribe Transcribe Vocabulary Filter API
  slug: amazon-transcribe-vocabulary-filter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-transcribe/openapi/amazon-transcribe-vocabulary-filter-api-openapi.yml
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
- host: transcribe.amazonaws.com
  https: false
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Amazon Transcribe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Transcribe, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Transcribe
provider_slug: amazon-transcribe
slug: amazon-transcribe-domain-security
source_filename: amazon-transcribe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: transcribe.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/amazon-transcribe/security/amazon-transcribe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Audio Processing
- Machine Learning
- Speech Recognition
- Speech-to-Text
- Transcription
---
