---
api_specs:
- filename: amazon-redshift-metadata-api-openapi.yml
  format: yaml
  label: Amazon Redshift Metadata API
  slug: amazon-redshift-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-redshift/refs/heads/main/openapi/amazon-redshift-metadata-api-openapi.yml
- filename: amazon-redshift-result-retrieval-api-openapi.yml
  format: yaml
  label: Amazon Redshift Result Retrieval API
  slug: amazon-redshift-result-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-redshift/refs/heads/main/openapi/amazon-redshift-result-retrieval-api-openapi.yml
- filename: amazon-redshift-statement-execution-api-openapi.yml
  format: yaml
  label: Amazon Redshift Statement Execution API
  slug: amazon-redshift-statement-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-redshift/refs/heads/main/openapi/amazon-redshift-statement-execution-api-openapi.yml
- filename: amazon-redshift-statement-management-api-openapi.yml
  format: yaml
  label: Amazon Redshift Statement Management API
  slug: amazon-redshift-statement-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-redshift/refs/heads/main/openapi/amazon-redshift-statement-management-api-openapi.yml
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
- host: redshift.amazonaws.com
  https: false
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: docs.aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amazon Redshift Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Redshift, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Redshift
provider_slug: amazon-redshift
slug: amazon-redshift-domain-security
source_filename: amazon-redshift-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: redshift.amazonaws.com\n  https: false\n- host: docs.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-redshift/refs/heads/main/security/amazon-redshift-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Big Data
- Cloud
- Data Lake
- Data Warehouse
- ETL
- Machine-Learning
- Serverless
- SQL
---
