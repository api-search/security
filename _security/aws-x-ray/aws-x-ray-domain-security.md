---
api_specs:
- filename: aws-x-ray-encryption-api-openapi.yml
  format: yaml
  label: AWS X-Ray Encryption API
  slug: aws-x-ray-encryption-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-x-ray/refs/heads/main/openapi/aws-x-ray-encryption-api-openapi.yml
- filename: aws-x-ray-groups-api-openapi.yml
  format: yaml
  label: AWS X-Ray Groups API
  slug: aws-x-ray-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-x-ray/refs/heads/main/openapi/aws-x-ray-groups-api-openapi.yml
- filename: aws-x-ray-insights-api-openapi.yml
  format: yaml
  label: AWS X-Ray Insights API
  slug: aws-x-ray-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-x-ray/refs/heads/main/openapi/aws-x-ray-insights-api-openapi.yml
- filename: aws-x-ray-sampling-api-openapi.yml
  format: yaml
  label: AWS X-Ray Sampling API
  slug: aws-x-ray-sampling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-x-ray/refs/heads/main/openapi/aws-x-ray-sampling-api-openapi.yml
- filename: aws-x-ray-service-graph-api-openapi.yml
  format: yaml
  label: AWS X-Ray Service Graph API
  slug: aws-x-ray-service-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-x-ray/refs/heads/main/openapi/aws-x-ray-service-graph-api-openapi.yml
- filename: aws-x-ray-tagresource-api-openapi.yml
  format: yaml
  label: AWS X-Ray TagResource API
  slug: aws-x-ray-tagresource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-x-ray/refs/heads/main/openapi/aws-x-ray-tagresource-api-openapi.yml
- filename: aws-x-ray-tags-api-openapi.yml
  format: yaml
  label: AWS X-Ray Tags API
  slug: aws-x-ray-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-x-ray/refs/heads/main/openapi/aws-x-ray-tags-api-openapi.yml
- filename: aws-x-ray-traces-api-openapi.yml
  format: yaml
  label: AWS X-Ray Traces API
  slug: aws-x-ray-traces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-x-ray/refs/heads/main/openapi/aws-x-ray-traces-api-openapi.yml
- filename: aws-x-ray-untagresource-api-openapi.yml
  format: yaml
  label: AWS X-Ray UntagResource API
  slug: aws-x-ray-untagresource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-x-ray/refs/heads/main/openapi/aws-x-ray-untagresource-api-openapi.yml
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
name: Aws X Ray Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AWS X-Ray, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AWS X-Ray
provider_slug: aws-x-ray
slug: aws-x-ray-domain-security
source_filename: aws-x-ray-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aws-x-ray/refs/heads/main/security/aws-x-ray-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Debugging
- Distributed Tracing
- Microservices
- Observability
---
