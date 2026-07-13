---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: score.dev
  spf: true
hosts:
- cert_expires: Aug 15 00:07:20 2026 GMT
  host: score.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Score Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Score, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Score
provider_slug: score
slug: score-domain-security
source_filename: score-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: score.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 00:07:20 2026 GMT\n  hsts: false\ndomains:\n- domain: score.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/score/refs/heads/main/security/score-domain-security.yml
summary_line: TLSv1.3
tags:
- Platform Engineering
- Cloud Native
- CNCF
- Workload Specification
- Kubernetes
- Docker
- Developer Experience
- Open Source
---
