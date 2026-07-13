---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: katacontainers.io
  spf: false
hosts:
- cert_expires: Sep 17 00:03:57 2026 GMT
  host: katacontainers.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kata Containers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kata Containers, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Kata Containers
provider_slug: kata-containers
slug: kata-containers-domain-security
source_filename: kata-containers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: katacontainers.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 00:03:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: katacontainers.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kata-containers/refs/heads/main/security/kata-containers-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Containers
- Isolation
- Kubernetes
- Open Source
- Security
- Virtual Machines
---
