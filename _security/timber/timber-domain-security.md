---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: vector.dev
  spf: false
hosts:
- cert_expires: Sep 28 23:59:59 2026 GMT
  host: vector.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Timber Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Timber, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Timber
provider_slug: timber
slug: timber-domain-security
source_filename: timber-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vector.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: vector.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/timber/refs/heads/main/security/timber-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Developer Tools
- Observability
- Logs
- Metrics
- Data Pipeline
- Logging
- Monitoring
- Open Source
- gRPC
- Rust
- Datadog
---
