---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: higress.io
  spf: false
hosts:
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: higress.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Higress Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Higress, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Higress
provider_slug: higress
slug: higress-domain-security
source_filename: higress-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: higress.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: higress.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/higress/refs/heads/main/security/higress-domain-security.yml
summary_line: TLSv1.3
tags:
- API Gateway
- Cloud Native
- Istio
- Kubernetes
---
