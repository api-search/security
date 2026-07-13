---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cert-manager.io
  spf: false
hosts:
- cert_expires: Sep  6 05:24:45 2026 GMT
  host: cert-manager.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cert Manager Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cert-Manager, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Cert-Manager
provider_slug: cert-manager
slug: cert-manager-domain-security
source_filename: cert-manager-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cert-manager.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 05:24:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cert-manager.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cert-manager/refs/heads/main/security/cert-manager-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Certificates
- Cloud Native
- Graduated
- Kubernetes
- Security
- TLS
---
