---
api_specs:
- filename: lambda-labs-asyncapi.yml
  format: yaml
  label: Lambda Inference API
  slug: inference-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/lambda-labs/refs/heads/main/asyncapi/lambda-labs-asyncapi.yml
- filename: lambda-labs-audit-events-api-openapi.yml
  format: yaml
  label: Lambda Audit Events API
  slug: lambda-labs-audit-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lambda-labs/refs/heads/main/openapi/lambda-labs-audit-events-api-openapi.yml
- filename: lambda-labs-fabric-api-openapi.yml
  format: yaml
  label: Lambda Fabric API
  slug: lambda-labs-fabric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lambda-labs/refs/heads/main/openapi/lambda-labs-fabric-api-openapi.yml
- filename: lambda-labs-filesystems-api-openapi.yml
  format: yaml
  label: Lambda Filesystems API
  slug: lambda-labs-filesystems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lambda-labs/refs/heads/main/openapi/lambda-labs-filesystems-api-openapi.yml
- filename: lambda-labs-firewalls-api-openapi.yml
  format: yaml
  label: Lambda Firewalls API
  slug: lambda-labs-firewalls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lambda-labs/refs/heads/main/openapi/lambda-labs-firewalls-api-openapi.yml
- filename: lambda-labs-images-api-openapi.yml
  format: yaml
  label: Lambda Images API
  slug: lambda-labs-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lambda-labs/refs/heads/main/openapi/lambda-labs-images-api-openapi.yml
- filename: lambda-labs-instances-api-openapi.yml
  format: yaml
  label: Lambda Instances API
  slug: lambda-labs-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lambda-labs/refs/heads/main/openapi/lambda-labs-instances-api-openapi.yml
- filename: lambda-labs-regions-api-openapi.yml
  format: yaml
  label: Lambda Regions API
  slug: lambda-labs-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lambda-labs/refs/heads/main/openapi/lambda-labs-regions-api-openapi.yml
- filename: lambda-labs-ssh-keys-api-openapi.yml
  format: yaml
  label: Lambda SSH keys API
  slug: lambda-labs-ssh-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lambda-labs/refs/heads/main/openapi/lambda-labs-ssh-keys-api-openapi.yml
- filename: lambda-labs-support-tickets-api-openapi.yml
  format: yaml
  label: Lambda Support Tickets API
  slug: lambda-labs-support-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lambda-labs/refs/heads/main/openapi/lambda-labs-support-tickets-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lambda.ai
  spf: true
hosts:
- cert_expires: Sep 25 02:35:14 2026 GMT
  host: lambda.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 06:14:15 2026 GMT
  host: cloud.lambda.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 06:00:59 2026 GMT
  host: docs.lambda.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lambda Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lambda, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lambda
provider_slug: lambda-labs
slug: lambda-labs-domain-security
source_filename: lambda-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lambda.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 02:35:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cloud.lambda.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 06:14:15 2026 GMT\n  hsts: null\n- host: docs.lambda.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 06:00:59 2026 GMT\n  hsts: false\ndomains:\n- domain: lambda.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lambda-labs/refs/heads/main/security/lambda-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Cloud
- Cluster
- Compute
- GPU
- Inference
- Machine-Learning
---
