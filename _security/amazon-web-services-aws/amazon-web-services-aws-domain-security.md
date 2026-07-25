---
api_specs:
- filename: amazon-web-services-aws-amazon-ec2-api-api-openapi.yml
  format: yaml
  label: Amazon Web Services (AWS) Amazon EC2 API API
  slug: amazon-web-services-aws-amazon-ec2-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-web-services-aws/refs/heads/main/openapi/amazon-web-services-aws-amazon-ec2-api-api-openapi.yml
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
name: Amazon Web Services Aws Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Web Services (AWS), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Web Services (AWS)
provider_slug: amazon-web-services-aws
slug: amazon-web-services-aws-domain-security
source_filename: amazon-web-services-aws-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: ec2.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: null\n- host: s3.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-web-services-aws/refs/heads/main/security/amazon-web-services-aws-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Artificial Intelligence
- Cloud Computing
- Computing
- Containers
- Databases
- Devops
- Iaas
- Infrastructure
- Machine Learning
- Networking
- Paas
- Platform As A Service
- Security
- Serverless
- Storage
---
