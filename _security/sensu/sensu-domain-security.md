---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sensu.io
  spf: true
hosts:
- cert_expires: Oct  8 23:14:51 2026 GMT
  host: sensu.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 23:41:15 2026 GMT
  host: docs.sensu.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sensu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sensu, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Sensu
provider_slug: sensu
slug: sensu-domain-security
source_filename: sensu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sensu.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:14:51 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.sensu.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:41:15 2026 GMT\n  hsts: false\ndomains:\n- domain: sensu.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sensu/refs/heads/main/security/sensu-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Monitoring
- Observability
- Infrastructure
- DevOps
- Metrics
- Events
- Alerting
- Monitoring as Code
- Kubernetes
---
