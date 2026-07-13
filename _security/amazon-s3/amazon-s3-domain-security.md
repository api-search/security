---
api_specs:
- filename: amazon-s3-rest-api-openapi.yml
  format: yaml
  label: Amazon S3 REST API
  slug: amazon-s3-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/openapi/amazon-s3-rest-api-openapi.yml
- filename: amazon-s3-control-api-openapi.yml
  format: yaml
  label: Amazon S3 Control API
  slug: amazon-s3-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/openapi/amazon-s3-control-api-openapi.yml
- filename: amazon-s3-tables-api-openapi.yml
  format: yaml
  label: Amazon S3 Tables API
  slug: amazon-s3-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/openapi/amazon-s3-tables-api-openapi.yml
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
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: s3.amazonaws.com
  hsts: null
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
name: Amazon S3 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon S3, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon S3
provider_slug: amazon-s3
slug: amazon-s3-domain-security
source_filename: amazon-s3-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: s3.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: null\n- host: docs.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/security/amazon-s3-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Archive
- Backup
- Cloud Storage
- Data Storage
- Object Storage
- Scalable Storage
---
