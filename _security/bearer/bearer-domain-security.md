---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bearer.com
  spf: true
hosts:
- cert_expires: Sep 29 15:56:19 2026 GMT
  host: www.bearer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bearer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bearer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bearer
provider_slug: bearer
slug: bearer-domain-security
source_filename: bearer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bearer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 15:56:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bearer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bearer/refs/heads/main/security/bearer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Infrastructure Saas
- Application Security
- Static Analysis
- SAST
- Code Security
- Data Privacy
- Developer Tools
- CLI
---
