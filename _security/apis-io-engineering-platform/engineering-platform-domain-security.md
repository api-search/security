---
api_specs:
- filename: aws-s3-openapi-original.yml
  format: yaml
  label: Amazon S3
  slug: aws-s3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-search/engineering-platform/refs/heads/main/openapi/aws-s3-openapi-original.yml
- filename: aws-lambda-openapi-original.yml
  format: yaml
  label: AWS Lambda
  slug: aws-lambda
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-search/engineering-platform/refs/heads/main/openapi/aws-lambda-openapi-original.yml
- filename: aws-api-gateway-openapi-original.yml
  format: yaml
  label: AWS API Gateway
  slug: aws-api-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-search/engineering-platform/refs/heads/main/openapi/aws-api-gateway-openapi-original.yml
- filename: aws-rds-openapi-original.yml
  format: yaml
  label: AWS RDS
  slug: aws-rds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-search/engineering-platform/refs/heads/main/openapi/aws-rds-openapi-original.yml
- filename: aws-iam-openapi-original.yml
  format: yaml
  label: AWS IAM
  slug: aws-iam
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-search/engineering-platform/refs/heads/main/openapi/aws-iam-openapi-original.yml
- filename: microsoft-cognitive-web-search-openapi-original.yml
  format: yaml
  label: Microsoft Bing Search
  slug: microsoft-bing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-search/engineering-platform/refs/heads/main/openapi/microsoft-cognitive-web-search-openapi-original.yml
- filename: postman-openapi-original.yml
  format: yaml
  label: Postman
  slug: postman
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-search/engineering-platform/refs/heads/main/openapi/postman-openapi-original.yml
- filename: cloudflare-openapi-original.yml
  format: yaml
  label: Cloudflare
  slug: cloudflare
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-search/engineering-platform/refs/heads/main/openapi/cloudflare-openapi-original.yml
- filename: github-openapi-original.yml
  format: yaml
  label: GitHub
  slug: github
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-search/engineering-platform/refs/heads/main/openapi/github-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: apis.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
hosts:
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: developer.apis.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: docs.aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- host: r275xc9bmd.execute-api.us-east-1.amazonaws.com
  https: false
kind: domain-security
layout: security
method: probed
name: Engineering Platform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for APIs.io Engineering Platform, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: APIs.io Engineering Platform
provider_slug: apis-io-engineering-platform
slug: engineering-platform-domain-security
source_filename: engineering-platform-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.apis.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: false\n- host: docs.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: r275xc9bmd.execute-api.us-east-1.amazonaws.com\n  https: false\ndomains:\n- domain: apis.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apis-io-engineering-platform/refs/heads/main/security/engineering-platform-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- APIs.io
- Engineering
- Platform
---
