---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: stackmachine.com
  spf: false
hosts:
- cert_expires: Sep  7 12:19:17 2026 GMT
  host: docs.stackmachine.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: api.stackmachine.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Stack Machine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stack Machine, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Stack Machine
provider_slug: stack-machine
slug: stack-machine-domain-security
source_filename: stack-machine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.stackmachine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 12:19:17 2026 GMT\n  hsts: false\n- host: api.stackmachine.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: stackmachine.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stack-machine/refs/heads/main/security/stack-machine-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Infrastructure
- Serverless
- WebAssembly
- Edge Compute
- AI Applications
- GraphQL
- Platform as a Service
- Deployment
- Hosting
- DNS
- Databases
---
