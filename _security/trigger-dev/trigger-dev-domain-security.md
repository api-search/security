---
api_specs:
- filename: trigger-dev-management-openapi.yml
  format: yaml
  label: Trigger.dev Management API
  slug: trigger-dev-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trigger-dev/refs/heads/main/openapi/trigger-dev-management-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: trigger.dev
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: your-self-hosted-instance.com
  spf: false
hosts:
- cert_expires: Sep 13 03:06:55 2026 GMT
  host: trigger.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 23:59:59 2026 GMT
  host: api.trigger.dev
  hsts: true
  hsts_max_age: 3153600000
  https: true
  tls_version: TLSv1.3
- host: your-self-hosted-instance.com
  https: false
kind: domain-security
layout: security
method: probed
name: Trigger Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trigger.dev, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Trigger.dev
provider_slug: trigger-dev
slug: trigger-dev-domain-security
source_filename: trigger-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trigger.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 03:06:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.trigger.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 3153600000\n- host: your-self-hosted-instance.com\n  https: false\ndomains:\n- domain: trigger.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: your-self-hosted-instance.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trigger-dev/refs/heads/main/security/trigger-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Developer-First
- Workflow Automation
- Background Jobs
- Durable Execution
- TypeScript
- AI Agents
- Realtime
- Open Source
---
