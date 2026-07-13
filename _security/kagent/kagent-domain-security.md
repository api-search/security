---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kagent.dev
  spf: false
hosts:
- cert_expires: Sep 27 16:29:09 2026 GMT
  host: kagent.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kagent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for kagent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: kagent
provider_slug: kagent
slug: kagent-domain-security
source_filename: kagent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kagent.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 16:29:09 2026 GMT\n  hsts: false\ndomains:\n- domain: kagent.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kagent/refs/heads/main/security/kagent-domain-security.yml
summary_line: TLSv1.3
tags:
- AI Agents
- Cloud Native
- DevOps
- Framework
- Kubernetes
---
