---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dchq.io
  spf: false
hosts:
- cert_expires: Aug 21 05:01:39 2026 GMT
  host: dchq.io
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dchq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DCHQ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: DCHQ
provider_slug: dchq
slug: dchq-domain-security
source_filename: dchq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dchq.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 21 05:01:39 2026 GMT\n  hsts: false\ndomains:\n- domain: dchq.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dchq/refs/heads/main/security/dchq-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Containers
- Docker
- Container Management
- Cloud Automation
- DevOps
- Application Deployment
- PaaS
---
