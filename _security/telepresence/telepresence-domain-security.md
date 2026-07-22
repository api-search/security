---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: telepresence.io
  spf: false
hosts:
- cert_expires: Aug 18 17:03:55 2026 GMT
  host: telepresence.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Telepresence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Telepresence, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Telepresence
provider_slug: telepresence
slug: telepresence-domain-security
source_filename: telepresence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: telepresence.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 17:03:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: telepresence.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telepresence/refs/heads/main/security/telepresence-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- CNCF
- Developer Tools
- Kubernetes
- Local Development
- Microservices
- Open Source
---
