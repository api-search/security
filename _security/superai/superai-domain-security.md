---
api_specs:
- filename: superai-flows-openapi-original.json
  format: json
  label: SuperAI Flows API
  slug: superai-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superai/refs/heads/main/openapi/superai-flows-openapi-original.json
description: ''
domains:
- caa:
  - 0 iodef "mailto:engineering@super.ai"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: super.ai
  spf: true
hosts:
- cert_expires: Sep 28 10:27:12 2026 GMT
  host: docs.flows.super.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 09:32:29 2026 GMT
  host: flows.super.ai
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Superai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Super.ai, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Super.ai
provider_slug: superai
slug: superai-domain-security
source_filename: superai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.flows.super.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 10:27:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: flows.super.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 09:32:29 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: super.ai\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:engineering@super.ai\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superai/refs/heads/main/security/superai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Enterprise Software
- Intelligent Document Processing
- Document Processing
- Workflow Orchestration
- Automation
- Human In The Loop
- Artificial Intelligence
- REST API
---
