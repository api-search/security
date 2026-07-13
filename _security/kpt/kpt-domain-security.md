---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kpt.dev
  spf: true
hosts:
- cert_expires: Sep 30 09:03:45 2026 GMT
  host: kpt.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kpt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kpt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Kpt
provider_slug: kpt
slug: kpt-domain-security
source_filename: kpt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kpt.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 09:03:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kpt.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kpt/refs/heads/main/security/kpt-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Configuration Management
- GitOps
- Infrastructure as Code
- Kubernetes
---
