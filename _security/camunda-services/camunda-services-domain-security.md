---
api_specs:
- filename: camunda-services-apis-tools-openapi-generated.yml
  format: yaml
  label: Camunda Services apis tools API
  slug: apis-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda-services/refs/heads/main/openapi/_ae-authored/camunda-services-apis-tools-openapi-generated.yml
- filename: camunda-services-core-openapi-generated.yml
  format: yaml
  label: Camunda Services core API
  slug: core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda-services/refs/heads/main/openapi/_ae-authored/camunda-services-core-openapi-generated.yml
- filename: camunda-services-self-managed-openapi-generated.yml
  format: yaml
  label: Camunda Services self managed API
  slug: self-managed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda-services/refs/heads/main/openapi/_ae-authored/camunda-services-self-managed-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: camunda.com
  spf: true
hosts:
- cert_expires: Dec 20 12:20:25 2026 GMT
  host: camunda.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Camunda Services Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Camunda Services, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Camunda Services
provider_slug: camunda-services
slug: camunda-services-domain-security
source_filename: camunda-services-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: camunda.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 12:20:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: camunda.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/camunda-services/refs/heads/main/security/camunda-services-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Workflow
- BPMN
- DMN
- Automation
---
