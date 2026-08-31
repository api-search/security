---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: restate.dev
  spf: true
hosts:
- cert_expires: Aug 31 21:22:25 2026 GMT
  host: restate.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 04:33:44 2026 GMT
  host: docs.restate.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Restate Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Restate, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Restate
provider_slug: restate-dev
slug: restate-dev-domain-security
source_filename: restate-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: restate.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 21:22:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.restate.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 04:33:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: restate.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/restate-dev/refs/heads/main/security/restate-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Agents
- Durable Execution
- Durable Workflows
- Event-Driven
- Kafka
- Microservice Orchestration
- Orchestration
- ProCode_API_Composition
- Resilience
- Sagas
- Self-Hosting
- Service Protocol
- State Machines
- Stateful Services
- Step Functions
- Virtual Objects
- Workflows
- XState
---
