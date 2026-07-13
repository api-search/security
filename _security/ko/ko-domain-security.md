---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ko.build
  spf: false
hosts:
- cert_expires: Sep 28 02:51:21 2026 GMT
  host: ko.build
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ko Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ko, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Ko
provider_slug: ko
slug: ko-domain-security
source_filename: ko-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ko.build\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 02:51:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: ko.build\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ko/refs/heads/main/security/ko-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Build Tools
- Container Images
- Containers
- Go
- Kubernetes
---
