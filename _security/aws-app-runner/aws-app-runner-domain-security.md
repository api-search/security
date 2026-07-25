---
api_specs:
- filename: aws-app-runner-auto-scaling-api-openapi.yml
  format: yaml
  label: AWS App Runner Auto Scaling API
  slug: aws-app-runner-auto-scaling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/openapi/aws-app-runner-auto-scaling-api-openapi.yml
- filename: aws-app-runner-aws-app-runner-api-api-openapi.yml
  format: yaml
  label: AWS App Runner AWS App Runner API API
  slug: aws-app-runner-aws-app-runner-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/openapi/aws-app-runner-aws-app-runner-api-api-openapi.yml
- filename: aws-app-runner-connections-api-openapi.yml
  format: yaml
  label: AWS App Runner Connections API
  slug: aws-app-runner-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/openapi/aws-app-runner-connections-api-openapi.yml
- filename: aws-app-runner-custom-domains-api-openapi.yml
  format: yaml
  label: AWS App Runner Custom Domains API
  slug: aws-app-runner-custom-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/openapi/aws-app-runner-custom-domains-api-openapi.yml
- filename: aws-app-runner-deleteservice-api-openapi.yml
  format: yaml
  label: 'AWS App Runner #DeleteService API'
  slug: aws-app-runner-deleteservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/openapi/aws-app-runner-deleteservice-api-openapi.yml
- filename: aws-app-runner-deployments-api-openapi.yml
  format: yaml
  label: AWS App Runner Deployments API
  slug: aws-app-runner-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/openapi/aws-app-runner-deployments-api-openapi.yml
- filename: aws-app-runner-describeservice-api-openapi.yml
  format: yaml
  label: 'AWS App Runner #DescribeService API'
  slug: aws-app-runner-describeservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/openapi/aws-app-runner-describeservice-api-openapi.yml
- filename: aws-app-runner-listservices-api-openapi.yml
  format: yaml
  label: 'AWS App Runner #ListServices API'
  slug: aws-app-runner-listservices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/openapi/aws-app-runner-listservices-api-openapi.yml
- filename: aws-app-runner-observability-api-openapi.yml
  format: yaml
  label: AWS App Runner Observability API
  slug: aws-app-runner-observability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/openapi/aws-app-runner-observability-api-openapi.yml
- filename: aws-app-runner-pauseservice-api-openapi.yml
  format: yaml
  label: 'AWS App Runner #PauseService API'
  slug: aws-app-runner-pauseservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/openapi/aws-app-runner-pauseservice-api-openapi.yml
- filename: aws-app-runner-resumeservice-api-openapi.yml
  format: yaml
  label: 'AWS App Runner #ResumeService API'
  slug: aws-app-runner-resumeservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/openapi/aws-app-runner-resumeservice-api-openapi.yml
- filename: aws-app-runner-updateservice-api-openapi.yml
  format: yaml
  label: 'AWS App Runner #UpdateService API'
  slug: aws-app-runner-updateservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/openapi/aws-app-runner-updateservice-api-openapi.yml
- filename: aws-app-runner-vpc-api-openapi.yml
  format: yaml
  label: AWS App Runner VPC API
  slug: aws-app-runner-vpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/openapi/aws-app-runner-vpc-api-openapi.yml
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
kind: domain-security
layout: security
method: probed
name: Aws App Runner Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AWS App Runner, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AWS App Runner
provider_slug: aws-app-runner
slug: aws-app-runner-domain-security
source_filename: aws-app-runner-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/security/aws-app-runner-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CI/CD
- Containers
- Deployment
- Microservices
- Serverless
---
