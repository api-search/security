---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coinremitter.com
  spf: true
hosts:
- cert_expires: Sep  2 16:41:33 2026 GMT
  host: coinremitter.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coinremitter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coinremitter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Coinremitter
provider_slug: coinremitter
slug: coinremitter-domain-security
source_filename: coinremitter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coinremitter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 16:41:33 2026 GMT\n  hsts: false\ndomains:\n- domain: coinremitter.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinremitter/refs/heads/main/security/coinremitter-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cryptocurrency
- Public APIs
---
