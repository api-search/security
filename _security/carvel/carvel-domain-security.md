---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: carvel.dev
  spf: false
hosts:
- cert_expires: Oct  4 02:58:13 2026 GMT
  host: carvel.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Carvel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carvel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Carvel
provider_slug: carvel
slug: carvel-domain-security
source_filename: carvel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carvel.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 02:58:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: carvel.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carvel/refs/heads/main/security/carvel-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- CLI
- Configuration
- Containers
- Deployment
- GitOps
- Kubernetes
- Package Management
- Templating
---
