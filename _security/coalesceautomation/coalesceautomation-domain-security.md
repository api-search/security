---
api_specs:
- filename: coalesceautomation-coalesceautomation-api-api-openapi.yml
  format: yaml
  label: Coalesceautomation Coalesceautomation API
  slug: coalesceautomation-coalesceautomation-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coalesceautomation/refs/heads/main/openapi/coalesceautomation-coalesceautomation-api-api-openapi.yml
- filename: coalesceautomation-environments-api-openapi.yml
  format: yaml
  label: Coalesceautomation Environments API
  slug: coalesceautomation-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coalesceautomation/refs/heads/main/openapi/coalesceautomation-environments-api-openapi.yml
- filename: coalesceautomation-projects-api-openapi.yml
  format: yaml
  label: Coalesceautomation Projects API
  slug: coalesceautomation-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coalesceautomation/refs/heads/main/openapi/coalesceautomation-projects-api-openapi.yml
- filename: coalesceautomation-public-api-openapi.yml
  format: yaml
  label: Coalesceautomation Public API
  slug: coalesceautomation-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coalesceautomation/refs/heads/main/openapi/coalesceautomation-public-api-openapi.yml
- filename: coalesceautomation-scheduler-api-openapi.yml
  format: yaml
  label: Coalesceautomation Scheduler API
  slug: coalesceautomation-scheduler-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coalesceautomation/refs/heads/main/openapi/coalesceautomation-scheduler-api-openapi.yml
- filename: coalesceautomation-workspaces-api-openapi.yml
  format: yaml
  label: Coalesceautomation Workspaces API
  slug: coalesceautomation-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coalesceautomation/refs/heads/main/openapi/coalesceautomation-workspaces-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coalesce.io
  spf: true
hosts:
- cert_expires: Jan  6 18:58:45 2027 GMT
  host: coalesce.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Coalesceautomation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coalesceautomation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Coalesceautomation
provider_slug: coalesceautomation
slug: coalesceautomation-domain-security
source_filename: coalesceautomation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coalesce.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 18:58:45 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: coalesce.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coalesceautomation/refs/heads/main/security/coalesceautomation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Platform
- Automation
- Metadata
- Cloud Integration
- Artificial Intelligence
- San Francisco
---
