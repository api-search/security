---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: antic.xyz
  spf: false
hosts:
- cert_expires: Aug  4 06:57:18 2026 GMT
  host: www.antic.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Antic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Antic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Antic
provider_slug: antic
slug: antic-domain-security
source_filename: antic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.antic.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  4 06:57:18 2026 GMT\n  hsts: false\ndomains:\n- domain: antic.xyz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/antic/refs/heads/main/security/antic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Crypto
---
