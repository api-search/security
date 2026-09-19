---
api_specs:
- filename: cloudflare-openapi-original.yml
  format: yaml
  label: Cloudflare API
  slug: cloudflare
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engineering-platform/refs/heads/main/openapi/_original/cloudflare-openapi-original.yml
- filename: github-openapi-original.yml
  format: yaml
  label: GitHub REST API
  slug: github
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engineering-platform/refs/heads/main/openapi/_original/github-openapi-original.yml
- filename: postman-openapi-original.yml
  format: yaml
  label: Postman API
  slug: postman
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engineering-platform/refs/heads/main/openapi/_original/postman-openapi-original.yml
- filename: aws-api-gateway-openapi-original.yml
  format: yaml
  label: Amazon API Gateway
  slug: aws-api-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engineering-platform/refs/heads/main/openapi/_original/aws-api-gateway-openapi-original.yml
- filename: aws-iam-openapi-original.yml
  format: yaml
  label: AWS Identity and Access Management
  slug: aws-iam
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engineering-platform/refs/heads/main/openapi/_original/aws-iam-openapi-original.yml
- filename: aws-lambda-openapi-original.yml
  format: yaml
  label: AWS Lambda
  slug: aws-lambda
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engineering-platform/refs/heads/main/openapi/_original/aws-lambda-openapi-original.yml
- filename: microsoft-cognitive-news-search-openapi-original.yml
  format: yaml
  label: Bing News Search API
  slug: microsoft-cognitive-news-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engineering-platform/refs/heads/main/openapi/_original/microsoft-cognitive-news-search-openapi-original.yml
- filename: microsoft-cognitive-video-search-openapi-original.yml
  format: yaml
  label: Bing Video Search API
  slug: microsoft-cognitive-video-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engineering-platform/refs/heads/main/openapi/_original/microsoft-cognitive-video-search-openapi-original.yml
- filename: microsoft-cognitive-web-search-openapi-original.yml
  format: yaml
  label: Bing Web Search API
  slug: microsoft-cognitive-web-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engineering-platform/refs/heads/main/openapi/_original/microsoft-cognitive-web-search-openapi-original.yml
- filename: aws-rds-openapi-original.yml
  format: yaml
  label: Amazon Relational Database Service
  slug: aws-rds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engineering-platform/refs/heads/main/openapi/aws-rds-openapi-original.yml
- filename: aws-s3-openapi-original.yml
  format: yaml
  label: Amazon Simple Storage Service
  slug: aws-s3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engineering-platform/refs/heads/main/openapi/aws-s3-openapi-original.yml
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
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Engineering Platform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for APIs.io Engineering Platform, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: APIs.io Engineering Platform
provider_slug: engineering-platform
slug: engineering-platform-domain-security
source_filename: engineering-platform-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.apis.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: false\n- host: docs.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: r275xc9bmd.execute-api.us-east-1.amazonaws.com\n  https: false\ndomains:\n- domain: apis.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/engineering-platform/refs/heads/main/security/engineering-platform-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- APIs.io
- Engineering
- Platform
---
