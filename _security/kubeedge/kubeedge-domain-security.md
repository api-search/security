---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kubeedge.io
  spf: true
hosts:
- cert_expires: Aug 23 07:57:41 2026 GMT
  host: kubeedge.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kubeedge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KubeEdge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: KubeEdge
provider_slug: kubeedge
slug: kubeedge-domain-security
source_filename: kubeedge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kubeedge.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 07:57:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kubeedge.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kubeedge/refs/heads/main/security/kubeedge-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Cloud Native
- Edge Computing
- Graduated
- IoT
- Kubernetes
---
