---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: kubernetes.io
  spf: true
hosts:
- cert_expires: Sep 11 09:13:55 2026 GMT
  host: kubernetes.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kubectl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kubectl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Kubectl
provider_slug: kubectl
slug: kubectl-domain-security
source_filename: kubectl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kubernetes.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 09:13:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kubernetes.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kubectl/refs/heads/main/security/kubectl-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Command Line Interface
- Infrastructure CLI
---
