---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cni.dev
  spf: false
hosts:
- cert_expires: Oct  2 15:07:58 2026 GMT
  host: www.cni.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cni Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Container Network Interface (CNI), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Container Network Interface (CNI)
provider_slug: cni
slug: cni-domain-security
source_filename: cni-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cni.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 15:07:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cni.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cni/refs/heads/main/security/cni-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Cloud Native
- Containers
- Incubating
- Kubernetes
- Networking
- Plugins
---
