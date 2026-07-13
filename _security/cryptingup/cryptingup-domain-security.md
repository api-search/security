---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cryptingup.com
  spf: true
hosts:
- cert_expires: Aug 26 19:33:14 2026 GMT
  host: www.cryptingup.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cryptingup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CryptingUp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CryptingUp
provider_slug: cryptingup
slug: cryptingup-domain-security
source_filename: cryptingup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cryptingup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 19:33:14 2026 GMT\n  hsts: null\ndomains:\n- domain: cryptingup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cryptingup/refs/heads/main/security/cryptingup-domain-security.yml
summary_line: TLSv1.3
tags:
- Cryptocurrency
- Public APIs
---
