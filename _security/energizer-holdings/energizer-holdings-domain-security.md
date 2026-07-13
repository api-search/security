---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: energizer.com
  spf: true
hosts:
- cert_expires: Aug 10 12:57:13 2026 GMT
  host: www.energizer.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: developer.energizer.com
  https: false
- host: api.energizer.com
  https: false
kind: domain-security
layout: security
method: probed
name: Energizer Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Energizer Holdings, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Energizer Holdings
provider_slug: energizer-holdings
slug: energizer-holdings-domain-security
source_filename: energizer-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.energizer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 12:57:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.energizer.com\n  https: false\n- host: api.energizer.com\n  https: false\ndomains:\n- domain: energizer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/energizer-holdings/refs/heads/main/security/energizer-holdings-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Consumer Products
- Batteries
---
