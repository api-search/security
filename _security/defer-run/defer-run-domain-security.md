---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: defer.run
  spf: false
hosts:
- cert_expires: Aug 27 14:25:00 2026 GMT
  host: www.defer.run
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Defer Run Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Defer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Defer
provider_slug: defer-run
slug: defer-run-domain-security
source_filename: defer-run-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.defer.run\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 14:25:00 2026 GMT\n  hsts: null\ndomains:\n- domain: defer.run\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/defer-run/refs/heads/main/security/defer-run-domain-security.yml
summary_line: TLSv1.3
tags:
- Background Jobs
- Asynchronous Processing
- Job Queues
- Serverless
- Node.js
- TypeScript
- Workflow Orchestration
- Cron
- Durable Execution
- Developer Tools
- Defunct
- Y Combinator
---
