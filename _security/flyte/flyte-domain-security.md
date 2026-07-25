---
api_specs:
- filename: flyte-dataproxy-api-openapi.yml
  format: yaml
  label: Flyte DataProxy API
  slug: flyte-dataproxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flyte/refs/heads/main/openapi/flyte-dataproxy-api-openapi.yml
- filename: flyte-events-api-openapi.yml
  format: yaml
  label: Flyte Events API
  slug: flyte-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flyte/refs/heads/main/openapi/flyte-events-api-openapi.yml
- filename: flyte-executions-api-openapi.yml
  format: yaml
  label: Flyte Executions API
  slug: flyte-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flyte/refs/heads/main/openapi/flyte-executions-api-openapi.yml
- filename: flyte-launchplans-api-openapi.yml
  format: yaml
  label: Flyte LaunchPlans API
  slug: flyte-launchplans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flyte/refs/heads/main/openapi/flyte-launchplans-api-openapi.yml
- filename: flyte-matchableattributes-api-openapi.yml
  format: yaml
  label: Flyte MatchableAttributes API
  slug: flyte-matchableattributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flyte/refs/heads/main/openapi/flyte-matchableattributes-api-openapi.yml
- filename: flyte-namedentities-api-openapi.yml
  format: yaml
  label: Flyte NamedEntities API
  slug: flyte-namedentities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flyte/refs/heads/main/openapi/flyte-namedentities-api-openapi.yml
- filename: flyte-nodeexecutions-api-openapi.yml
  format: yaml
  label: Flyte NodeExecutions API
  slug: flyte-nodeexecutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flyte/refs/heads/main/openapi/flyte-nodeexecutions-api-openapi.yml
- filename: flyte-projects-api-openapi.yml
  format: yaml
  label: Flyte Projects API
  slug: flyte-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flyte/refs/heads/main/openapi/flyte-projects-api-openapi.yml
- filename: flyte-taskexecutions-api-openapi.yml
  format: yaml
  label: Flyte TaskExecutions API
  slug: flyte-taskexecutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flyte/refs/heads/main/openapi/flyte-taskexecutions-api-openapi.yml
- filename: flyte-tasks-api-openapi.yml
  format: yaml
  label: Flyte Tasks API
  slug: flyte-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flyte/refs/heads/main/openapi/flyte-tasks-api-openapi.yml
- filename: flyte-version-api-openapi.yml
  format: yaml
  label: Flyte Version API
  slug: flyte-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flyte/refs/heads/main/openapi/flyte-version-api-openapi.yml
- filename: flyte-workflows-api-openapi.yml
  format: yaml
  label: Flyte Workflows API
  slug: flyte-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flyte/refs/heads/main/openapi/flyte-workflows-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: flyte.org
  spf: false
hosts:
- cert_expires: Aug 16 20:17:19 2026 GMT
  host: flyte.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 17:38:56 2026 GMT
  host: docs.flyte.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flyte Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flyte, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Flyte
provider_slug: flyte
slug: flyte-domain-security
source_filename: flyte-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flyte.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 20:17:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.flyte.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 17:38:56 2026 GMT\n  hsts: false\ndomains:\n- domain: flyte.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flyte/refs/heads/main/security/flyte-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- CNCF
- Data Orchestration
- Kubernetes
- Machine Learning
- Workflow Automation
---
