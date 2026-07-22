---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: blockvigil.com
  spf: true
hosts:
- cert_expires: Oct  9 19:00:27 2026 GMT
  host: blockvigil.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blockvigil Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BlockVigil, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: BlockVigil
provider_slug: blockvigil
slug: blockvigil-domain-security
source_filename: blockvigil-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blockvigil.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 19:00:27 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: blockvigil.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blockvigil/refs/heads/main/security/blockvigil-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Blockchain
- Web3
- Discontinued
- Portfolio
---
