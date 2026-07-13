---
api_specs:
- filename: unionai-openapi.yml
  format: yaml
  label: Union FlyteAdmin Projects API
  slug: flyteadmin-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unionai/refs/heads/main/openapi/unionai-openapi.yml
- filename: unionai-openapi.yml
  format: yaml
  label: Union FlyteAdmin Workflows API
  slug: flyteadmin-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unionai/refs/heads/main/openapi/unionai-openapi.yml
- filename: unionai-openapi.yml
  format: yaml
  label: Union FlyteAdmin Tasks API
  slug: flyteadmin-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unionai/refs/heads/main/openapi/unionai-openapi.yml
- filename: unionai-openapi.yml
  format: yaml
  label: Union FlyteAdmin Launch Plans API
  slug: flyteadmin-launch-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unionai/refs/heads/main/openapi/unionai-openapi.yml
- filename: unionai-openapi.yml
  format: yaml
  label: Union FlyteAdmin Executions API
  slug: flyteadmin-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unionai/refs/heads/main/openapi/unionai-openapi.yml
- filename: unionai-openapi.yml
  format: yaml
  label: Union Serverless
  slug: union-serverless
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unionai/refs/heads/main/openapi/unionai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: union.ai
  spf: true
hosts:
- cert_expires: Oct  3 06:10:37 2026 GMT
  host: www.union.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: <your-org>.app.union.ai
  https: false
- cert_expires: Oct 19 23:59:59 2026 GMT
  host: serverless.union.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unionai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Union.ai, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Union.ai
provider_slug: unionai
slug: unionai-domain-security
source_filename: unionai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.union.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 06:10:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: <your-org>.app.union.ai\n  https: false\n- host: serverless.union.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: union.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unionai/refs/heads/main/security/unionai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- AI
- ML
- Orchestration
- Workflows
- MLOps
- Flyte
- Serverless
---
