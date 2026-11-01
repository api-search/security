---
api_specs:
- filename: amazon-emr-clusters-api-openapi.yml
  format: yaml
  label: Amazon EMR Clusters API
  slug: amazon-emr-clusters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-clusters-api-openapi.yml
- filename: amazon-emr-auto-termination-policy-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Auto Termination Policy API
  slug: amazon-emr-auto-termination-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-auto-termination-policy-api-openapi.yml
- filename: amazon-emr-instance-fleet-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Instance Fleet API
  slug: amazon-emr-instance-fleet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-instance-fleet-api-openapi.yml
- filename: amazon-emr-instance-group-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Instance Group API
  slug: amazon-emr-instance-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-instance-group-api-openapi.yml
- filename: amazon-emr-managed-scaling-policy-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Managed Scaling Policy API
  slug: amazon-emr-managed-scaling-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-managed-scaling-policy-api-openapi.yml
- filename: amazon-emr-notebook-execution-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Notebook Execution API
  slug: amazon-emr-notebook-execution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-notebook-execution-api-openapi.yml
- filename: amazon-emr-operations-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Operations API
  slug: amazon-emr-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-operations-api-openapi.yml
- filename: amazon-emr-security-configuration-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Security Configuration API
  slug: amazon-emr-security-configuration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-security-configuration-api-openapi.yml
- filename: amazon-emr-session-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Session API
  slug: amazon-emr-session-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-session-api-openapi.yml
- filename: amazon-emr-step-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Step API
  slug: amazon-emr-step-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-step-api-openapi.yml
- filename: amazon-emr-studio-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Studio API
  slug: amazon-emr-studio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-studio-api-openapi.yml
- filename: amazon-emr-studio-session-mapping-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Studio Session Mapping API
  slug: amazon-emr-studio-session-mapping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-studio-session-mapping-api-openapi.yml
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
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: elasticmapreduce.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Amazon Emr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon EMR, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon EMR
provider_slug: amazon-emr
slug: amazon-emr-domain-security
source_filename: amazon-emr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: elasticmapreduce.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/amazon-emr/security/amazon-emr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Amazon Web Services
- Analytics
- Apache Spark
- Big Data
- Data Processing
- Hadoop
---
