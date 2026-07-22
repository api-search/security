---
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: false
  domain: lumigo.io
  spf: false
hosts:
- cert_expires: Oct  2 05:57:16 2026 GMT
  host: lumigo.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lumigo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lumigo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present.'
provider_name: Lumigo
provider_slug: lumigo
slug: lumigo-domain-security
source_filename: lumigo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lumigo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 05:57:16 2026 GMT\n  hsts: false\ndomains:\n- domain: lumigo.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lumigo/refs/heads/main/security/lumigo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Observability
- Monitoring
- Serverless
- Distributed Tracing
- OpenTelemetry
- AWS Lambda
- Microservices
- Logs
---
