---
api_specs:
- filename: aws-redshift-openapi.json
  format: json
  label: Amazon Redshift API
  slug: amazon-redshift-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/openapi/aws-redshift-openapi.json
- filename: aws-redshift-data-openapi.json
  format: json
  label: Amazon Redshift Data API
  slug: amazon-redshift-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/openapi/aws-redshift-data-openapi.json
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
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: docs.aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aws Redshift Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AWS Redshift, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AWS Redshift
provider_slug: aws-redshift
slug: aws-redshift-domain-security
source_filename: aws-redshift-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: docs.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/security/aws-redshift-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
---
