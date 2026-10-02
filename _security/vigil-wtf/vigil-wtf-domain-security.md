---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vigil.wtf
  spf: true
hosts:
- cert_expires: Nov  2 15:18:42 2026 GMT
  host: www.vigil.wtf
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Vigil Wtf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vigil, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vigil
provider_slug: vigil-wtf
slug: vigil-wtf-domain-security
source_filename: vigil-wtf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vigil.wtf\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 15:18:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: vigil.wtf\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vigil-wtf/refs/heads/main/security/vigil-wtf-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Monitoring
- AI Middleware
- Security
- Analytics
---
