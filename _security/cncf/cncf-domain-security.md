---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cncf.io
  spf: true
hosts:
- cert_expires: Aug 29 04:32:56 2026 GMT
  host: www.cncf.io
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: landscape.cncf.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cncf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CNCF, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CNCF
provider_slug: cncf
slug: cncf-domain-security
source_filename: cncf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cncf.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 04:32:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: landscape.cncf.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cncf.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cncf/refs/heads/main/security/cncf-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Native
- Containers
- Kubernetes
- Open Source
- Standards
---
