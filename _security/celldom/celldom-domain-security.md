---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: celldom.com
  spf: true
hosts:
- cert_expires: Dec 13 09:56:44 2026 GMT
  host: www.celldom.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Celldom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Celldom, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Celldom
provider_slug: celldom
slug: celldom-domain-security
source_filename: celldom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.celldom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 09:56:44 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: celldom.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/celldom/refs/heads/main/security/celldom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Single Cell
- Platform
- Drug Discovery
---
