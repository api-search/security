---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: granulate.io
  spf: true
hosts:
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: granulate.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Granulate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Granulate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Granulate
provider_slug: granulate
slug: granulate-domain-security
source_filename: granulate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: granulate.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: granulate.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/granulate/refs/heads/main/security/granulate-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Devops
- Performance
- Continuous Profiling
- Observability
- Optimization
- Kubernetes
- Intel
---
