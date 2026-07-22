---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: abc.xyz
  spf: true
hosts:
- cert_expires: Sep  4 08:18:54 2026 GMT
  host: abc.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alphabet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alphabet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Alphabet
provider_slug: alphabet
slug: alphabet-domain-security
source_filename: alphabet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: abc.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 08:18:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: abc.xyz\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alphabet/refs/heads/main/security/alphabet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Technology
- Search
- Advertising
- Cloud Computing
- AI
- Fortune 100
---
