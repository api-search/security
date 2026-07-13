---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: buoyant.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: linkerd.io
  spf: false
hosts:
- cert_expires: Sep 29 12:15:44 2026 GMT
  host: buoyant.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 15:31:59 2026 GMT
  host: linkerd.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Buoyant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Buoyant, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Buoyant
provider_slug: buoyant
slug: buoyant-domain-security
source_filename: buoyant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buoyant.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 12:15:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: linkerd.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 15:31:59 2026 GMT\n  hsts: false\ndomains:\n- domain: buoyant.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: linkerd.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buoyant/refs/heads/main/security/buoyant-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Observability
- Kubernetes
- Linkerd
- mTLS
- Observability
- Service Mesh
- Zero Trust
---
