---
description: ''
domains:
- caa:
  - 1 issue "letsencrypt.org"
  - 0 issue "trust-provider.com"
  dmarc: false
  dnssec: true
  domain: standardkernel.com
  spf: false
hosts:
- cert_expires: Oct 14 22:28:24 2026 GMT
  host: standardkernel.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Standard Kernel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Standard Kernel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Standard Kernel
provider_slug: standard-kernel
slug: standard-kernel-domain-security
source_filename: standard-kernel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: standardkernel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 22:28:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: standardkernel.com\n  dnssec: true\n  caa:\n  - 1 issue \"letsencrypt.org\"\n  - 0 issue \"trust-provider.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/standard-kernel/refs/heads/main/security/standard-kernel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- AI Infrastructure
- GPU
- Kernel Optimization
- Compilers
- Machine Learning
- Artificial Intelligence
---
