---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pathcrypto.com
  spf: true
hosts:
- cert_expires: Nov 13 04:12:01 2026 GMT
  host: www.pathcrypto.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Path Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Path, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Path
provider_slug: path
slug: path-domain-security
source_filename: path-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pathcrypto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 04:12:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pathcrypto.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/path/refs/heads/main/security/path-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cryptocurrency
- Financial Services
- Investment
- Portfolio Management
- SEC Registered
---
