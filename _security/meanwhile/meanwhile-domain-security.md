---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: meanwhile.bm
  spf: true
hosts:
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: meanwhile.bm
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Meanwhile Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meanwhile, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Meanwhile
provider_slug: meanwhile
slug: meanwhile-domain-security
source_filename: meanwhile-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: meanwhile.bm\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: meanwhile.bm\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meanwhile/refs/heads/main/security/meanwhile-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Crypto
- Bitcoin
- Insurance
- Life Insurance
- Fintech
- Bermuda
---
