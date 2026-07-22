---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: werf.io
  spf: false
hosts:
- cert_expires: Dec 11 14:59:19 2026 GMT
  host: werf.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Werf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Werf, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Werf
provider_slug: werf
slug: werf-domain-security
source_filename: werf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: werf.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 14:59:19 2026 GMT\n  hsts: false\ndomains:\n- domain: werf.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/werf/refs/heads/main/security/werf-domain-security.yml
summary_line: TLSv1.3
tags:
- CI/CD
- Deployment
- DevOps
- GitOps
- Kubernetes
- CNCF
- Helm
- Containers
- Open Source
---
