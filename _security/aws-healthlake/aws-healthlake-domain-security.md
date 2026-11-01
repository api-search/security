---
api_specs:
- filename: aws-healthlake-datastore-api-openapi.yml
  format: yaml
  label: AWS HealthLake Datastore API
  slug: aws-healthlake-datastore-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aws-healthlake/openapi/aws-healthlake-datastore-api-openapi.yml
- filename: aws-healthlake-export-api-openapi.yml
  format: yaml
  label: AWS HealthLake Export API
  slug: aws-healthlake-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aws-healthlake/openapi/aws-healthlake-export-api-openapi.yml
- filename: aws-healthlake-import-api-openapi.yml
  format: yaml
  label: AWS HealthLake Import API
  slug: aws-healthlake-import-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aws-healthlake/openapi/aws-healthlake-import-api-openapi.yml
- filename: aws-healthlake-tags-api-openapi.yml
  format: yaml
  label: AWS HealthLake Tags API
  slug: aws-healthlake-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aws-healthlake/openapi/aws-healthlake-tags-api-openapi.yml
- filename: aws-healthlake-data-transformation-job-api-openapi.yml
  format: yaml
  label: AWS HealthLake Healthlake Data Transformation Job API
  slug: aws-healthlake-data-transformation-job-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aws-healthlake/openapi/aws-healthlake-data-transformation-job-api-openapi.yml
- filename: aws-healthlake-data-transformation-profile-api-openapi.yml
  format: yaml
  label: AWS HealthLake Healthlake Data Transformation Profile API
  slug: aws-healthlake-data-transformation-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aws-healthlake/openapi/aws-healthlake-data-transformation-profile-api-openapi.yml
- filename: aws-healthlake-operations-api-openapi.yml
  format: yaml
  label: AWS HealthLake Healthlake Operations API
  slug: aws-healthlake-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aws-healthlake/openapi/aws-healthlake-operations-api-openapi.yml
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
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: docs.aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: healthlake.us-east-1.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Aws Healthlake Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AWS HealthLake, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AWS HealthLake
provider_slug: aws-healthlake
slug: aws-healthlake-domain-security
source_filename: aws-healthlake-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: docs.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: healthlake.us-east-1.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/aws-healthlake/security/aws-healthlake-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- FHIR
- Health Data
- Clinical Data
- HIPAA
- Interoperability
- Natural Language Processing
- Medical
- HL7
---
