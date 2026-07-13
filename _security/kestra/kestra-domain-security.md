---
api_specs:
- filename: open-source
  format: yaml
  label: Kestra Flows API
  slug: flows-api
  spec_type: OpenAPI
  url: https://kestra.io/docs/api-reference/open-source
- filename: open-source
  format: yaml
  label: Kestra Executions API
  slug: executions-api
  spec_type: OpenAPI
  url: https://kestra.io/docs/api-reference/open-source
- filename: open-source
  format: yaml
  label: Kestra Namespaces API
  slug: namespaces-api
  spec_type: OpenAPI
  url: https://kestra.io/docs/api-reference/open-source
- filename: open-source
  format: yaml
  label: Kestra Key-Value Store API
  slug: kv-store-api
  spec_type: OpenAPI
  url: https://kestra.io/docs/api-reference/open-source
- filename: open-source
  format: yaml
  label: Kestra Namespace Files API
  slug: namespace-files-api
  spec_type: OpenAPI
  url: https://kestra.io/docs/api-reference/open-source
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: kestra.io
  spf: true
hosts:
- cert_expires: Aug 19 19:26:46 2026 GMT
  host: kestra.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kestra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kestra, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Kestra
provider_slug: kestra
slug: kestra-domain-security
source_filename: kestra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kestra.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 19:26:46 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: kestra.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kestra/refs/heads/main/security/kestra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Automation
- Data Pipelines
- Event-Driven
- Orchestration
- Workflows
---
