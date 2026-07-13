---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: sozu.io
  spf: true
hosts:
- cert_expires: Sep 22 08:21:18 2026 GMT
  host: www.sozu.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: docs.sozu.io
  https: false
kind: domain-security
layout: security
method: probed
name: Sozu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sozu, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Sozu
provider_slug: sozu
slug: sozu-domain-security
source_filename: sozu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sozu.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 08:21:18 2026 GMT\n  hsts: false\n- host: docs.sozu.io\n  https: false\ndomains:\n- domain: sozu.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sozu/refs/heads/main/security/sozu-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Proxy
- Reverse Proxy
- Load Balancing
- Rust
- Open Source
---
