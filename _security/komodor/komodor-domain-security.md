---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: komodor.com
  spf: true
hosts:
- cert_expires: Sep 15 02:19:36 2026 GMT
  host: komodor.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: api.komodor.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Komodor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Komodor, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Komodor
provider_slug: komodor
slug: komodor-domain-security
source_filename: komodor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: komodor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 02:19:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.komodor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: komodor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/komodor/refs/heads/main/security/komodor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Kubernetes
- Observability
- SRE
- Troubleshooting
- DevOps
- Cloud Native
---
