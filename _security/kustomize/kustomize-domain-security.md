---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kustomize.io
  spf: false
hosts:
- cert_expires: Oct  6 19:33:49 2026 GMT
  host: kustomize.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kustomize Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kustomize, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Kustomize
provider_slug: kustomize
slug: kustomize-domain-security
source_filename: kustomize-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kustomize.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 19:33:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kustomize.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kustomize/refs/heads/main/security/kustomize-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Configuration Management
- Containers
- Infrastructure as Code
- Kubernetes
- YAML
---
