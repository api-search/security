---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Amazon EC2
  slug: amazon-ec2
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/ec2/2016-11-15/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Amazon S3
  slug: amazon-s3
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/s3/2006-03-01/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Amazon Lambda
  slug: amazon-lambda
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/lambda/2015-03-31/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Amazon DynamoDB
  slug: amazon-dynamodb
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/dynamodb/2012-08-10/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Amazon RDS
  slug: amazon-rds
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/rds/2014-10-31/openapi.yaml
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
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: ec2.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: s3.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aws Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Web Services (AWS), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Web Services (AWS)
provider_slug: aws
slug: aws-domain-security
source_filename: aws-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: ec2.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: null\n- host: s3.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aws/refs/heads/main/security/aws-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Computing
- IaaS
- Infrastructure
- PaaS
- Platform as a Service
- Serverless
---
