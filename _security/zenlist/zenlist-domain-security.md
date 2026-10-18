---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zenlist.com
  spf: true
hosts:
- cert_expires: Mar  3 23:59:59 2027 GMT
  host: zenlist.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zenlist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zenlist, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zenlist
provider_slug: zenlist
slug: zenlist-domain-security
source_filename: zenlist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zenlist.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: zenlist.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenlist/refs/heads/main/security/zenlist-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Real Estate
- Home Search
- MLS
- RESO
- Brokerage Software
---
