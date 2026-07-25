---
api_specs:
- filename: harness-organizations-api-openapi.yml
  format: yaml
  label: Harness Organizations API
  slug: harness-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harness/refs/heads/main/openapi/harness-organizations-api-openapi.yml
- filename: harness-pipeline-execution-api-openapi.yml
  format: yaml
  label: Harness Pipeline Execution API
  slug: harness-pipeline-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harness/refs/heads/main/openapi/harness-pipeline-execution-api-openapi.yml
- filename: harness-pipelines-api-openapi.yml
  format: yaml
  label: Harness Pipelines API
  slug: harness-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harness/refs/heads/main/openapi/harness-pipelines-api-openapi.yml
- filename: harness-projects-api-openapi.yml
  format: yaml
  label: Harness Projects API
  slug: harness-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harness/refs/heads/main/openapi/harness-projects-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: harness.io
  spf: true
hosts:
- cert_expires: Sep 18 00:03:41 2026 GMT
  host: developer.harness.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 22:40:00 2026 GMT
  host: apidocs.harness.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: app.harness.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Harness Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Harness, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Harness
provider_slug: harness
slug: harness-domain-security
source_filename: harness-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.harness.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 00:03:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidocs.harness.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 22:40:00 2026 GMT\n  hsts: false\n- host: app.harness.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: harness.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harness/refs/heads/main/security/harness-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- DevOps
- GitOps
- Internal Developer Portal
- Lifecycle
- Software Delivery
---
